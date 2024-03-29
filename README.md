This project is to keep track of my work at Horizontal. At the time of this writing, the project is divided into 2 sections; Resources & Worknotes. As time passes, the complexity of the organization of the project and resources increases, so this readme should document the overall process of building out this resource and documentation project.

For ease of navigability and to minimize the sizes of individual documents, the help of [markdown_helper](https://github.com/BurdetteLamar/markdown_helper) has been enlisted. For each of the main sections of this project, there is a ...-base.md file which has the includes in it. For example, if I run the following command:  

```markdown_helper include --pristine resources-base.md resources.md```

markdown_helper will make an uncommented (--pristine) version of resources.md based off of the resources-base.md file (which contains all of the includes). The structure of that terminal command is: call markdown_helper > tell it to include files > do not include comments > base file > output file

Also, take a look at the _config.yml file for some GitHub Pages configuration information.

There is a La Croíx counter on the main page of this site. If you click the La Croíx logo, you will be taken to a page that displays how many cans of La Croíx I have drank visually, in cans.