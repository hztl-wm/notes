<details>
<summary>Tenant and Site Creation</summary>
<br />  

Right-click on ```Content``` node and a dropdown menu will appear. From here, follow ```Insert > Tenant```. If your site will have numerous sub-sites, you can either create a ```Tenant Folder``` which can house multiple ```Tenants```, or you can create a ```Tenant``` which can also house multiple ```Tenants```. Each Tenant has a set of Data Templates, which are stored in the Templates section which you can share within a Tenant. You can also share Rendering Variants, Themes, and Media. Think first about how your organizational structure should be reflected, then click the button to make the thing.  

When you right click on ```Content``` then select ```Insert > Tenant``` a Tenant creation wizard will appear. It's magical. It is a single-step wizard, so it's not really that magical. But you should give your Tenant a name according to the naming conventions you have agreed upon with your client and or team, and additionally, you can select which of the Modules you may need for your Tenant.

Once you have created your Tenant, it will appear along the following path; ```sitecore > Content > *new_tenant_you_created*```. If you select your tenant, you will be able to explore all of the relevant paths for your tenant, available modules, shared site information. Once you have created this tenant, you will notice that in some places along your sitecore folder tree, that some new folders have been created. i.e. ```sitecore > Templates *new_tenant_you_created*```. In that folder there will be a bunch of Data Templates. Same for the Media Library, ```sitecore > Media Library > Project > *new_tenant_you_created*```.

Next, right-click on the ```*new_tenant_you_created*```, and you will see a menu similar to when you right-click on the ```Content``` in your folder tree. Under ```Insert``` there are options to create a Site, Site Folder, or Insert From Template. Click ```Insert > Site``` and the Site wizard will load. This wizard is more complex than the first one we met, this is a 4-tabbed wizard. He will ask you about General, Modules, Theme, and Grid. Be ready.

Under General > Site name, tell the 4-tabbed wizard the name of your site. You will do this by clicking into the Site name field, then using the keyboard to type the name of your site. i.e. My Super Awesome Sitecore SXA Website. In the Host name field, you will have to tell the 4-tabbed wizard the URL for your website, but it will also need to be bound and that's a thing that BED people do, so as the presenter does, just skip that $***. In the Virtual folder field, the 4-tabbed wizard is curious if you would like to store your files anywhere other than the site root. Just leave it alone. Same with the Language dropdown; if you want anything other than English, select that, otherwise, leave it alone.

Moving on to the second tab in our 4-tabbed wizard, Modules, here you can select the modules that you may want preconfigured for your site. This time, think about what Modules you actually want, because sitecore will make all of them if you want, but that's a lot of time and data which you may not need to waste or use. If you happen to make an improper selection or miss a Module, you can fix that later on.

Welcome to the third tab in our 4-tabbed wizard, Theme. You can create a new theme by clicking the checkbox labeled *Create a new theme*. There also exists a default theme called *Wireframe*. Check the *Create a new theme* checkbox and in the *New theme name* input field, tell the 4-tabbed wizard the name of your new theme.

And... we've made it to the fourth and final tab in our 4-tabbed wizard, Grid. By default, there are THREE grid options; Bootstrap, Foundation, and Grid 960. Just go with Bootstrap and click that little blue Ok button in the bottom-right corner of the 4-tabbed wizard and the new *My Super Awesome Sitecore SXA Website* site will generate. It may take a while, go get a La Croíx or take a nap. Do NOT do anything else or the 4-tabbed wizard will destroy your computer and most of the internet.

Phew, you dodged a something by following directions well. Click the little blue Close button and now you will see your *My Super Awesome Sitecore SXA Website* site underneath your previously created Tenant, i.e. ```sitecore > Content > *new_tenant_you_created* > My Super Awesome Sitecore SXA Website```. Inside of your My Super Awesome Sitecore SXA Website in the folder tree, you can see a whole bunch of folders that have been made by the 4-tabbed wizard for you! He made; Home, Media, Data, Presentation, and Settings folders! Home stores all of your webpages, Media stores media, Data stores all of the different Modules you selected earlier (these will act as a datasource for your website), Presentation stores the different files that control how your website looks and behaves, and finally Settings allows you to change a bunch of settings for your site (404 page, 500 server error page control lives here). Under ```sitecore > Content > *new_tenant_you_created* > My Super Awesome Sitecore SXA Website > Settings > Site Grouping > My Super Awesome Sitecore SXA Website```, you can find the settings that you defined with the 4-tabbed wizard *General* tab.

A Site will share datasources with its tenant, but you will have control over theme and a virtual folder for the site will exist independent of the tenant. If you should ever need to delete your site, you can rihght-click on the site name in the folder tree and under *Scripts*, click the *Remove site* option. This will run a script that removes all of the folders which are specific to the site which you would like to remove. The *Are you sure you want to delete My Super Awesome Sitecore SXA Website?* wizard will launch to confirm your decision. If you are certain, you may click the blue *OK* button, if you would like to thank this wizard for saving you from making an egregious error, click the grey *Cancel* button, and the wizards disappearance will serve as acknowledgement of both your thanks and your error. There is a similar option available for Tenants that you wish to remove from your sitecore instance. Follow the above steps and meet the wizard.

If you had deselected a module when running though any of the wizards you have met before *(either the tenant one-step wizard, or the site 4-tabbed wizard)* and would like to add a module to them, right-click on the name of the site or tenant and under the *Scripts* menu, there is a script called *Add Site module*. Click that. The Add site module wizard will appear to help you in your search to add modules. If you have made any custom modules for sitecore and placed them in your sitecore instance, they would be available in the add module wizard if you had not selected them when making a tenant or site.

</details>

<details>
<summary>SXA Partial and Page Design Basics</summary>
<br />  

*Within SXA, you can use partial and page designs to create your UX layout.*

After datasource architecture, partial and page designs is a likely first step. Follow this path ```sitecore > Content > *my_tenant_name* > *my_site_name* > Presentation > Page || Partial Designs```. Partial Designs, i.e. a Header or Footer, are combined to create a Page Design. Right-click on ```Partial Designs``` then find ```Insert > Partial Design```. In the partial design wizard, give your partial design a name, i.e. Header, then click ok. Your new partial design will appear in the folder tree, right-click on that then click ```Experience Editor```, this will open the *Experience Editor*.

Within the *Experience Editor* you can drag and drop components into your partial design. In the *Experience Editor*, you will see (in the main part of the screen) a field that looks like a canvas (grey and white checkboard patterned), this is where the components for your partial design will go. There is a *header*, a *main*, and a *footer* for each partial design and when the page is rendered, these sections will be rendered in that order. For example, if you are making a Header component, but place the components for the partial design in a section that is not the header, then your Header Partial Design will not render in the header of your page.

![alt text](assets/images/SXA-Experience-Editor-Canvas.png "SXA Experience Editor Canvas")
*SXA Experience Editor Canvas. The alternating white and blue squares are highlighting the *main* section of the partial design canvas area.*

To add a component to the Header, drag the *Navigation* component from the right-hand side of the *Experience Editor* to the header section of the canvas. The *Navigation* component is nested under the *NAVIGATION* category of available components. Once the *Navigation* component is in the header section of the canvas, a toolbar for that component will appear (as seen below).

![alt text](assets/images/SXA-Experience-Editor-Navigation-Component.png "SXA Experience Editor Canvas")
*SXA Experience Editor Navigation Component placed in header of Design Partial, toolbar active.*

On the right-side of the toolbar for your placed component, there is a dropdown menu, labeled *More*, underneath which are additional options for your component. Click *More*, then click *Edit component properties* to open the wizard.

</details>