# Descriptions of Panel.ini Editor Settings

This open source project was created by the Plesk team. It encourages Plesk administrators to help each other by filling 
in missing descriptions of Panel.ini Editor settings.

## What is Panel.Ini Editor?

By default, the `panel.ini file` has a number of preconfigured settings with useful comments in front of each section. 
It is sufficient to get a brief grasp of basic `panel.ini` settings but not enough for something more challenging. 

![alt text](https://github.com/Eevee-chan/ext-panel-ini-editor-descriptions/blob/master/Img/1.bmp)

So, in Panel.ini Editor 3.1.0, we have added the "Description" column so that each `panel.ini` setting can now have a description. 
Each setting can, but few have…

## How come? I want all settings to have descriptions!

We added descriptions for a number of useful settings, but filling in each description is not our target.

## Got it. How can I fill in descriptions myself?

You can edit descriptions right inside Panel.ini Editor. Type whatever you like, because these descriptions are saved on your server only.

However, if you feel that your descriptions are too good to keep to yourself, you can share them with other Panel.Ini Editor users (we would be really grateful if you do!).

## How do I make my descriptions available to other users?

1. Add a branch to the [ext-panel-ini-editor-descriptions](https://github.com/plesk/ext-panel-ini-editor-descriptions) repository.
2. Pick a language to write descriptions in:
    * To write in English, edit the `en-US.json` file inside the branch.
    * To write in another language, create a new JSON file inside the cloned repository (unless the file for the same language already exists). 
    [Name the JSON file according to the languages codes here](https://docs.plesk.com/en-US/onyx/localization-guide/appendix-locale-codes.64474/). 
    
        For example, if you want to add descriptions in German and no one has created the JSON file for the German locale yet, create `de-DE.json` and edit it.
3. Add descriptions complying with the JSON file structure:

    ````json
    {
      "section1": {
        "setting1": "description",
        "setting2": "description"
      },
      " section2": {
        "setting1": "description"
      }
    }
    ````

    For example, if you want to add a description for the `allowedIPs` setting,
        
    then the JSON entry will look like this:        

    ````json
    {
      "api": {
        "allowedIPs": "description"
      }
    }
    ````

4. Commit the changes to your branch and then create a pull request to the [ext-panel-ini-editor-descriptions repository](https://github.com/plesk/ext-panel-ini-editor-descriptions).

## What’s Next?

We regularly review pull requests and approve good ones. Each released version of Panel.Ini Editor will include these approved descriptions. 
When Panel.ini Editor is updated, users will receive a bunch of new descriptions of `panel.ini` settings. 

## Acknowledgment 

Our best contributors are:
