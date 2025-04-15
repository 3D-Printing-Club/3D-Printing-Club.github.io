# 3DPC-Website

This is the official 3DPC website hosted at [purdue3dpc.org](https://purdue3dpc.org/). 
Here is an overview of how the website is working currently:
1. Mobirise is used as a free visual code editor that has a paywall to modify the code directly. However, free extensions exist to get around this by adding their own code editing buttons, which work great. More info is in the "How To Get Started" section below.
2. Mobirise is connected to github with an access token, which will then allow you to directly push changes to this repo through the mobirise gui, and have them automatically deployed with CI/CD.
3. Our domain registration and DNS is done on cloudflare. This domain must be renewed for $10/year or going to purdue3dpc.org will not work. It is currently set to expire Oct. 18, 2025.
4. The website connects to a firestore database that will dynamically load the events and gallery pages. The gallery images are saved on google drive in the "Website Gallery" folder.
5. These documents and images are uploaded by a discord bot that has its own repo called 3dpc-bot, so see the README there for more information on this.

------
## How To Get Started
Here are detailed instructions covering everything you need to know to develop the website. 
1. Follow the directions [here](https://mobirise.com/help/start-362.html) to download and install the mobirise.
2. Once you have the app installed, clone the gh-pages branch of this repository by either downloading as zip or using `git clone`. Do this by first clicking the source control button in the top left and choosing 'gh-pages', then click the green button and follow one of the options.
3. Next, open mobirise, go to the sites tab, and click 'import mobirise site' under 'create new site'. Then choose the project.mobirise file in the downloaded repository.
4. Next, you will want to connect the site to github. First, enable github publishing by going to Account > App Settings, and enabling 'Publish to Github Pages'.
5. Then fill in the github login and token below this slider. The login is "Purdue-3D-Printing-Club" and the token is in officer secrets (under "Website Mobirise-Github Personal Access Token). Feel free to dm me (Andrew Thompson) on Discord if you need this token and can't get access to it for whatever reason.
6. Now you can exit this menu and click the publish button in the top right. Select Github Pages, and fill in the link below this with Purdue-3D-Printing-Club.github.io/3DPC-Website (The ".github.io/" part is static)
7. Make sure to enable "publish changes only" so that you aren't overwriting other work.
8. Your github connection should be all ready now, so you can click publish and it will make a commit on this github repository and deploy the website with your changes.

Now here's some more information about how to actually develop the website:
9. You will need the following free code editor extension to directly modify code blocks: go [here](https://witsec.nl/extension-code-editor.html) and download the code editor extension. This will give you the .mbrext file, which you will need to import by going to Extensions > Import (top left). Select the mbrext file in the popup, then click "import anyway". 
10. This will add a wrench icon when you hover over a code block. Clicking the wrench icon will open a code editor to add your own custom code. Be careful, however, because any errors in here could cause the block to bug out and you might not be able to edit it again. I recommend that you save backups frequently when you directly edit the code in this way.
11. That's pretty much it! Mobirise is quite intuitive to use. you can add and remove blocks and edit the text inline. There are also some other useful extensions on witsec's website [here] (https://witsec.nl/index.html#our-extensions). Follow the same procedure as the code editor to import them.





