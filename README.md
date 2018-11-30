# ubicomp-on-a-budget
A repository collecting all the bits and pieces of the local ubicomp experiments


## TODO
1. DO A VIDEO GUIDE FOR USING WEBSTRATES FOR DEVELOPMENT
2. DO ONE THAT WITH FILESYSTEM

# Guides

## Installing webstrates file system (WFS)

### On Windows

1. [Install Nodejs](https://nodejs.org/en/)
    1. Check Environmental Variables:
    2. Go to Control Panel > System and Security > System > Advanced system Settings
    3. Click on Environmental Variables
    4. In the User varables for <user>, mark 'Path' and click 'edit'
    5. Add nodejs default path (if not there): `C:\Program Files\nodejs`
    6. Add npm default path (if not there): `C:\Users\<user>\AppData\Roaming\npm`
    7. Ok everything and exit
    8. Open Command Prompt and type `node -v`to confirm that nodejs is installed (out: v10.14.*)
2. [Install Github Desktop](https://desktop.github.com/)
3. [Install webstrate-file-system](https://github.com/Webstrates/file-system)
    1. Click 'Clone or download' and click 'Open in Desktop'
    2. Open Command Prompt and go to webstrate-file-system in the Github folder `cd C:\Users\<user>\Documents\Github\file-system`
    3. Install with `npm install`
4. Connect to the webstrate server with the file system tool
    1. Open Command Prompt and go to webstrate-file-system in the Github folder `cd C:\Users\<user>\Documents\Github\file-system`2
    2. type in prompt `node index.js --id=test-installaton --host=proxemics.cs.au.dk`
5. Make an edit
    1. Open a text editor of choice (make sure it opdates the file in view if it's update on the file system)
    2. Add a random message in the `body` tag, e.g. `Hello, what an awesome guide -- thank you Henrik!`
  
    


Follow this guide for installing the WFS:

https://github.com/Webstrates/file-system

Run this command to connect to our experimental server

`wfs --id=[your_webstrateId] --host=proxemics.cs.au.dk`
