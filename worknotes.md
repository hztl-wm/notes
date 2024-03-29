---
title: Daily Worknotes
---

The purpose of this document is to keep a running record of my daily activities at [Horizontal](http://horizontalintegration.com)  
These are mostly notes related to ongoing projects

<details>
<summary>2019</summary>
<details>
<summary>October</summary>
<br>

10/7

*Finished the SXA training series'. Moving back to Accessibility in JavaScript. Also have CSS manifest for ab to pore over as well*

Accessibility in JavaScript @ 30mins left. Have nice notes on Medium and the forked repo on github with comments all over the code as it comes in the workshop. Had a nice conversation with my surpervisor about BED and FED working together and how it doesn't always work well, lessons learned, and how to move forward.

10/6

Thought I had no meetings, so I decided to WFH. At 08:30 a PM reached out and asked if I was coming to Scrum. Yes? But it wasn't on my calendar. Spent the day going through the SXA Rendering Variant set of videos. There's a lot of little things to consider when setting up a project on such a large platform, but if you can make the pieces smaller and smaller and understand how it all comes together, then it should be manageable. The break point between FED and BED is still unclear, but I think the SXA series is mostly geared towards FEDs, Content Authors, and Marketeers, so all the BED things are somewhere else?

10/4

I am now on ab half-time and have the other half of my time to do other things? There is plenty to keep me busy, I am finishing up SXA training, which is documented on the resources page. After that, I still have to finish Accessibility in JavaScript AND HR had sent over some trainings for me to complete. Yay.

Stackla update: FED won

10/3

Well well well... I used up all my allocation for mwt by noon yesterday and then started in on ab sxa business. We had the ab stand-up this morning and I was the only one who had cleared my plate to start in on the SXA trainings... Today I reported in for the mwt standup that I had passed off my ticket and it was in a good place, but after a day with Stackla, guess who won? Stackla... Anyway, I wrote up a bunch more notes about the SXA training, that's over on my Resources page. I also figured out how to use markdown_helper to organize (complicate) my work here a bit more. SXA is pretty WYSIWYG(y), and it is yet unclear how BED and FED will work together using this platform, but I hope it proves useful and worth all the trouble!

---

10/2

*had to get out of Stackla and mwt. Only had half time this week for that and ab, so mwt is out for the week. Moving on to ab, started learning sxa thangs.*

* mwt 56 - pip product reviews - made some good progress on this. Got the base set for the layout of the page in mobile and desktop views, but the functional requirements are not yet met. Having to pass this back to the other FED on the project to implement, but would have needed their help on this component nonetheless. Oh JavaScript, there is so much to learn. Stackla wins.

me: 1, stackla: 2

---

10/1

*spent the whole day in Stackla. I have nothing but inappropriate things to write...*

* mwt 56 - pip product reviews - the fight continues. I did find that we may have been using the wrong base template for the social card widget on Stackla. Switched to another template and have found a greater deal of flexibility working with this thing, but I'm still giving Stackla a point for the day, because they win.

me: 1, stackla: 1  

</details>
<details>
<summary>September</summary>
<br>

9/30

*finally received some comments on a PR submitted by BED for mwt... it was requested that I change a lot of element classes to better suit BEM. ugh BEM*

* mwt 97 - pip video component - as the note above mentions, we finally got some feedback on this PR and most of the requested changes came from how I had set up the names of the things. Not BEMmy enough... that's what she said. Complaints aside, I don't mind. It has been interesting to get familiar with another development teams processes, structure, and (in this case) naming conventions.

* mwt 56 - pip product reviews - fighting this thing still. Got the 3 types of review cards up on a template page. After the BEM attack I got from the video component, I can only expect I will get some similar feedback on this one, but my main goal is to get it built for now.

me: 1, stackla: 0

---

9/27

*client launched the things we've been working on and it was a happy moment for all involved. today was an oktoberfest celebration*

* mwt 56 - pip product reviews - spent the day working with a service called [Stackla](https://developer.stackla.com). Something the client uses for part of their site. Has a code editor not unlike Codepen, but the embed code provides an iframe which means that you have to get as much ```CSS``` and ```JavaScript``` into the code editor because it's not easy (impossible?) to reach into the iframe... Spent a bit of time figuring out how to provide a div with an ```SVG``` background-image and compiled those resources over on my...Resource page. Also learned that I remembered the ```HTML``` code for a non-breaking space. Amazing. ```&nbsp;``` Here's what the ```SVG``` code looks like:

<details>
<summary>It's horrific, you've been warned</summary>
<br>

```scss
.instagram {
	background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2038%2038%22%3E%3Cpath%20fill%3D%22%230a0a0a%22%20fill-rule%3D%22evenodd%22%20d%3D%22M19%200c10.5%200%2019%208.5%2019%2019s-8.5%2019-19%2019S0%2029.5%200%2019%208.5%200%2019%200z%22%20clip-rule%3D%22evenodd%22%2F%3E%3Cpath%20fill%3D%22%23fff%22%20fill-rule%3D%22evenodd%22%20d%3D%22M18.8%207.8c-2.7%200-3%200-4.1.1-1%200-1.8.2-2.4.5-.6.3-1.2.6-1.7%201.1-.5.5-.9%201.1-1.1%201.7-.2.6-.4%201.3-.5%202.4v4.1c0%202.7%200%203%20.1%204.1%200%201%20.2%201.8.5%202.4.3.6.6%201.2%201.1%201.7.5.5%201.1.9%201.7%201.1.6.2%201.3.4%202.4.5%201%200%201.4.1%204.1.1%202.7%200%203%200%204.1-.1%201%200%201.8-.2%202.4-.5.6-.3%201.2-.6%201.7-1.1.5-.5.9-1.1%201.1-1.7.2-.6.4-1.3.5-2.4%200-1%20.1-1.4.1-4.1%200-2.7%200-3-.1-4.1%200-1-.2-1.8-.5-2.4-.3-.6-.6-1.2-1.1-1.7-.5-.5-1.1-.9-1.7-1.1-.6-.2-1.3-.4-2.4-.5-1.2-.1-1.5-.1-4.2-.1m0%201.8c2.6%200%202.9%200%204%20.1%201%200%201.5.2%201.8.3.5.2.8.4%201.1.7.3.3.6.7.7%201.1.1.3.3.9.3%201.8%200%201%20.1%201.3.1%204%200%202.6%200%202.9-.1%204%200%201-.2%201.5-.3%201.8-.2.5-.4.8-.7%201.1-.3.3-.7.6-1.1.7-.3.1-.9.3-1.8.3-1%200-1.3.1-4%20.1s-2.9%200-4-.1c-1%200-1.5-.2-1.8-.3-.5-.2-.8-.4-1.1-.7-.3-.3-.6-.7-.7-1.1-.1-.3-.3-.9-.3-1.8%200-1-.1-1.3-.1-4%200-2.6%200-2.9.1-4%200-1%20.2-1.5.3-1.8.2-.5.4-.8.7-1.1.3-.3.7-.6%201.1-.7.3-.1.9-.3%201.8-.3%201.1-.1%201.4-.1%204-.1m.2%2011.1c-1.8%200-3.2-1.5-3.2-3.2%200-1.8%201.5-3.2%203.2-3.2%201.8%200%203.2%201.5%203.2%203.2%200%201.8-1.4%203.2-3.2%203.2m0-8.2c-2.8%200-5%202.2-5%205s2.2%205%205%205%205-2.2%205-5-2.2-5-5-5m6%200c0%20.6-.4%201-1%201s-1-.4-1-1%20.4-1%201-1%201%20.4%201%201%22%20clip-rule%3D%22evenodd%22%2F%3E%3C%2Fsvg%3E");
	width: 38px;
	height: 38px;
	background-size: contain;
	margin-right: 10px;
}
```
</details>

Basically what is happening above is an ```SVG``` was exported from Illustrator, ran through a service that minimizes the code, then through a URL encoder. The links over at my [Resources](./resources.md) page are quite detailed in how this works. It was nice to find a workaround for the limitations that is [Stackla](https://developer.stackla.com).

me: 1, stackla: 0

---

9/26

Spent the day going over [Frontend Masters Accessibility in JavaScript](https://frontendmasters.com/courses/javascript-accessibility) course. Have been writing up notes [here](https://medium.com/@hztl_wm/accessibility-in-javascript-applications-8a0b01d8266f) and commenting on the codebase [here](https://github.com/hztl-wm/fem-js-a11y-workshop). I will be presenting my findings on Tuesday 10/1 during our bi-weekly FED team meeting.

*I also added a La Croix consumption counter to the main page of this little repo, becuase who doesn't love a good La Croix or 3?*

---

9/25

*fought with responsive ```SVG``` (I see you cw), attended 3 too many meetings, only drank 2 la croix*

* mwt 97 - pip video component - Another fun run-in with ```SVG```. Of course this needed to be responsive, so after tons of somethinging... here's what I ended up with:

<details>
<summary>Click to view my work of the day</summary>
<br>

```html
<div class="pip-video">
    <div class="media-gallery__img media-gallery__video video-link" data-video="" data-brightcovevideo="6076312645001" data-brightcoveplayer="r1tg8ngpM">
        <img src="image link removed to preserve client anonymity" alt="">
        <div class="pip-video__icon">
            <!-- <svg width="100%" height="100%" version="1.1" id="pip-video-play-button" xmlns="http://www.w3.org/2000/svg"
            x="0px" y="0px" viewBox="0 0 106 106" style="enable-background:new 0 0 106 106;" xml:space="preserve" preserveAspectRatio="xMinYMin">
            <path id="outline" class="st0" d="M53,105.5C24.1,105.5,0.5,81.9,0.5,53C0.5,24.1,24.1,0.5,53,0.5c28.9,0,52.5,23.6,52.5,52.5 C105.5,81.9,81.9,105.5,53,105.5z M53,3.5C25.7,3.5,3.5,25.7,3.5,53c0,27.3,22.2,49.5,49.5,49.5c27.3,0,49.5-22.2,49.5-49.5 C102.5,25.7,80.3,3.5,53,3.5z" fill="#33EB91"/>
            <path id="background" class="st1" d="M53,7c25.4,0,46,20.6,46,46S78.4,99,53,99S7,78.4,7,53S27.6,7,53,7z" fill="rgba(0,0,0,.5)"/>
            <path id="triangle" class="st2" d="M73,51.5L41,77.9V25.1L73,51.5z" fill="#ffffff"/>
            </svg> -->
        </div>
    </div>
</div>
<div id="modal-video" class="modal modal--video">
    <div class="pip-video modal__content">
        <div class="pip-video__video-wrapper">
            <video-js 
                data-account="" 
                data-embed="default" 
                data-player="" 
                data-video-id="" 
                style="height:auto; position:relative; width:100vw;"
                controls
            ></video-js>
        </div>
    </div>
</div>
```

```scss
.pip-video {
    width: 100%;
    margin: auto;
    position: relative;
    
    & .video-link::after {
        right: 0;
        top: 0;
        height: 100%;content: '';
        position: absolute;
        width: 100vw;
        background: -moz-linear-gradient(top, rgba(0,0,0,0) 80%, rgba(0,0,0,0.95) 100%); /* FF3.6+ */
        background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,rgba(0,0,0,0.95)), color-stop(100%,rgba(0,0,0,0))); /* Chrome,Safari4+ */
        background: -webkit-linear-gradient(top, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* Chrome10+,Safari5.1+ */
        background: -o-linear-gradient(top, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* Opera 11.10+ */
        background: -ms-linear-gradient(top, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* IE10+ */
        background: linear-gradient(to bottom, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* W3C */
    }
    
    & div > img {
        width: 100vw;
        height: auto;
        
    }

    &__icon {
        position: absolute;
        max-width: 12%;
        top: 40%;
        left: 44%;

        @media screen and (min-width: $tablet-min) {
            max-width: 6%;
            top: 40%;
            left: 47%;
        }
    }

}
```
</details>

---

9/24

*mwt merged repos, built and deployed the project in its current state. Lots of bugs knocked out, focus shifted to PIP (Product Information Page) Component production*

* mwt 99 - pip gallery component - Another new component build based off of the Sketch file provided by UX. Having become more familiar with the project structure, this was an easier build, but there were some interesting trip ups provided by flexbox. The major hiccups were uneven columns, an image that spanned 2 columns and rows, and gradient overlays. The following ```HTML``` and ```SCSS``` is how that was handled. Built for mobile first, the ```SCSS``` is what really drives the magic here. I hope the clients dev team doesn't mind my ```@mixin``` here because it helped to make the code more DRY.

<details>
<summary>Click to view my work of the day</summary>
<br>

```scss
@import ''; // link removed to preserve client anonymity
@mixin overlay-base {
    content: '';
    position: absolute;
    width: 100vw;
    background: -moz-linear-gradient(top, rgba(0,0,0,0) 80%, rgba(0,0,0,0.95) 100%); /* FF3.6+ */
    background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,rgba(0,0,0,0.95)), color-stop(100%,rgba(0,0,0,0))); /* Chrome,Safari4+ */
    background: -webkit-linear-gradient(top, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* Chrome10+,Safari5.1+ */
    background: -o-linear-gradient(top, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* Opera 11.10+ */
    background: -ms-linear-gradient(top, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* IE10+ */
    background: linear-gradient(to bottom, rgba(0,0,0,0) 80%,rgba(0,0,0,0.95) 100%); /* W3C */
}
.pip-gallery {
    width: 100vw;
    display: flex;
    position: relative;
    flex-wrap: wrap;
    @media screen and (min-width: $tablet-min) {
        flex-wrap: nowrap;
    }
    
    &__large-image {
        flex: 0 0 100vw;
        order: 1;
        @media screen and (min-width: $tablet-min) {
            flex: 0 0 66.66vw;
        }
        
        & img {
            width: 100%;
            z-index: -1;
        }
        
        &__overlay::after {
            @include overlay-base;
            left: 0;
            top: 0;
            height: 33.33%;
            @media screen and (min-width: $tablet-min) {
                height: 100%;
                width: 66.66vw;
            }
        }
    }
    
    &__small-image {
        flex: 0 0 100vw;
        flex-direction: unset;
        order: 2;
        @media screen and (min-width: $tablet-min) {
            flex: 0 0 33.33vw;
        }
        
        &__overlay-top::after {
            @include overlay-base;
            right: 0;
            top: 0;
            height: 67%;
            @media screen and (min-width: $tablet-min) {
                height: 50%;
                width: 33.33vw;
            }
        }
        &__overlay-bottom::after {
            @include overlay-base;
            right: 0;
            bottom: 0;
            height: 100%;
            @media screen and (min-width: $tablet-min) {
                height: 50%;
                width: 33.33vw;
            }
        }
        
        & img {
            width: 100%;
            z-index: -1;
        }
    }
}
```

```html
<section class="pip-gallery">
    <div class="pip-gallery__large-image">
        <div class="pip-gallery__large-image__overlay">
            <img src="/pip-gallery-1.png">
        </div>
    </div>
    <div class="pip-gallery__small-image">
        <div class="pip-gallery__small-image__overlay-top">
            <img src="/pip-gallery-2.png">
        </div>
        <div class="pip-gallery__small-image__overlay-bottom">
            <img src="/pip-gallery-3.png">
        </div>
    </div>
</section>
```
</details>

---

9/23

* mwt 91 - hero header component - UPDATE - I had this reviewed internally before passing it on. I neglected that this was a new component that needed to be fleshed out by BED before a PR was submitted, so my PR got abandoned ¯\_(ツ)_/¯ Not a big deal, more a matter of me learning the workflow a bit. BED got this knocked out and all looks good.

---

9/20

*mwt internal team having trouble with build and deployment*

* mwt 91 - hero header component - This is a new component build based off of a Sketch file provided by UX. I have had some trouble with the overall structure of the project, would probably have been useful to spend some time speaking with a dev who has worked on the project before just diving in. Exported and cleaned up an ```SVG```, built out ```HTML``` and ```SCSS``` for the component. Would like someone to review before I submit a PR. Can hopefully get that this Monday.

---

9/19

*Closed out remaining cw tickets.*  
*Working on mwt full time now.*

* mwt 185 - RTE Text Formatting - BED refused a classname from our markup which broke body copy styling. Additionally, styling was needed for `<strong>` text. I did that. Like this:

```scss
p {
    margin-top: 11px;
    strong {
        font-family: Helvetica Neue LT W01_83 Hv Ex,Helvetica Neue,Helvetica,Arial,sans-serif;
        // had to change the above to a variable *$helvetica83* that had been declared in a separate file
        text-transform: uppercase;
    }
}
```

* mwt 182 / 184 - Extra Whitespace - BED had reused a classname on an element which resulted in strange behavior. I added a new classname and relevant styling, but once implemented by BED, Sitecore adds spaces in a `<div>` with no content and the `:empty` pseudo-selector was unable to work. Thankfully, BED *was* able to write some logic that will conditionally render the `<div>` if there is content for it. Also had update the name of a file, because some FED had not done that causing the test page to be broken.

```scss
.flex-content-feature-accordion {
        display: flex;
        width: 100%;
        order: 3;
        &:empty {
            display: none;
        }
    }
```

* mwt 35 Tabbed Carousel - pushed yesterdays changes to dev

---

9/18

* mwt 35 Tabbed Carousel - this component (based off of [slick slider](https://kenwheeler.github.io/slick/)) was intended to be used stand-alone, but of course QA found a reason to use it twice on a page (maybe there is a genuine use case for this?). Needless to say, how the component was initally set up was targeting a class instead of a unique ID. Adding a data-target was able to solve the problem. The changes made are as follows:

*these were the changes made to the JavaScript*

```javascript
...
var $this = $(this); // this line already existed
var target = $this.data('target');

// inside of the slick slider settings

asNavFor: '#' + target,

// targets the unique id

...$('#' + target).slick...
```

*and these were the changes made to the HTML files*

```html
<div class="innovations-tabbed-view__items" id="1"> <!-- added the id -->
```

```html
<section class="innovations-tabbed-view" data-target="1"> <!-- added the data-target -->
```

---

9/17

* cw 6472 Chapter Component - add spacing to match spec `margin-bottom: 4rem;`
* cw 6462 Update search field to match specs - set `max-width` according to spec
* cw 6172 Update image specs for download asset component - generated new set of images and updated component markup

---

9/16

* cw 8239 Lazy loading - updated waypoint offset from 66% to 80%, elements above the fold should appear more readily
* cw 8266 Add button to Insights page render

---

9/13

* cw 8046 Header Utility Menu Display Issue - had to define width for .header-utilityNav item; was breaking to a new line
* cw 6058 Subscribe CTA - broken `::before` && `::after` - had to define pseudo element translateX positioning for devices below XS breakpoint
* cw 6462 Hero Search Input Size - updated width of search field, had initially placed the fix in the wrong file... specificity broke the 'fix', now it is fixed
* cw 7186 Multimedia Search Results Page - fix from yesterday has been pushed to QA, but the modal open mask covers the entire page now. CoveoSearchInterface put a `z-index` on the wrapper which overrode the modal `z-index`.

---

9/12

* cw 7813 Hero Page Title Card - Fixed min-height for event of no button (an optional element)
* cw 7186 Multimedia Search Results Page - Continues playing on modal close fix;

*podcasts were broken because BED did not use the unique classnames set for the two different podcast sources
videos were broken because Coveo loads after the video modal JS is init, added:*

```javascript
if (window.YT) { $(window).trigger('youTubePlayerApiReady'); }; &&
if (window.VidyardV4) { $(window).trigger('vidyardPlayerApiReady'); };
```

*triggers if element is found*

---

9/11

*Target class of '.coveo-query-summary-cancel-last' and change text to 'Try a different search term'*

```javascript
$('.coveo-query-summary-cancel-last').text('Try a different search term');
```

* cw 8047 Design and Implement CoveoQuerySummary CSS
* cw 8068 Hero Image & Video Cards SM / XS breakpoint fix
* cw 7813 Hero Page Title Card Image Size(s) fix

</details>
</details>
