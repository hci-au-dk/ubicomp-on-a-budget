# ubicomp-on-a-budget
A repository collecting all the bits and pieces of the local ubicomp experiments


## TODO
1. DO A VIDEO GUIDE FOR USING WEBSTRATES FOR DEVELOPMENT
2. DO ONE THAT WITH FILESYSTEM

# Guides

## Installing webstrates file system (WFS)

The webstrate file system requires git, Github Desktop (Windows) and nodejs/npm. 

### On Windows

1. [Install Nodejs](https://nodejs.org/en/)
2. [Install Git](https://git-scm.com/download/win)
3. Check the proper Environmental variables are set:
    1. Go to Control Panel > System and Security > System > Advanced system Settings
    2. Click on Environmental Variables
    3. Verify the following path variables exist in either User or System varibles:
        1. `C:\Program Files\nodejs\`
        2. `C:\Program Files\Git\cmd`
        3. [Possibly optional]`C:\Users\<user>\AppData\Roaming\npm`
4. Verify that both Git and Node is installed by running `git --version` and `node --version` in Command Prompt
3. [Install Github Desktop](https://desktop.github.com/)
4. [Install webstrate-file-system](https://github.com/Webstrates/file-system)
    1. Click 'Clone or download' and click 'Open in Desktop'
    2. Open Command Prompt and go to webstrate-file-system in the Github folder `cd C:\Users\<user>\Documents\Github\file-system`
    3. Install with `npm install`
5. Connect to the webstrate server with the file system tool
    1. Open Command Prompt and go to webstrate-file-system in the Github folder `cd C:\Users\<user>\Documents\Github\file-system`
    2. type in prompt `node index.js --id=test-installaton --host=proxemics.cs.au.dk`
6. Make an edit
    1. Open the file in a text editor of choice (make sure it opdates the file in view if it's update on the file system)
    2. Add a random message in the `body` tag, e.g. `Hello Henrik, what an awesome guide!`
  
    
### On Mac/Linux

1. [Install Nodejs](https://nodejs.org/en/)
2. [Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
3. [Install webstrate-file-system](https://github.com/Webstrates/file-system)
4. Verify that both Git and Node is installed by running `git --version` and `node --version` in Terminal
5. [Install webstrate-file-system](https://github.com/Webstrates/file-system)
    1. Install with `npm install -g webstrates-file-system`
6. Connect to the webstrate server with the file system tool
    1. Go to you desired code directory in terminal -- e.g.  `~/github/`
    2. type in prompt `wfs --id=test-installaton --host=proxemics.cs.au.dk`
7. Make an edit
    1. Open the file in a text editor of choice (make sure it opdates the file in view if it's update on the file system)
    2. Add a random message in the `body` tag, e.g. `Hello Henrik, what an awesome guide!`

## Developing web-applications with webstrate [Henrik's approach]
1. Design as much of your application in a local .html file
2. When ready to add "webstrates" copy/paste the contents of the local file into a webstrate (either using the file-system or in developer tool.

###  Things to be aware of
1. New code is not executed until refresh
2. Each client executes the javascript in a webstrate. This opens up for race conditions and other interesting issues when using `setInterval` or `setTimeout`  with DOM manipulation
3. The file-system tool can cause wierd syncronisation issues (primarily on Windows). If the file is suddenly reverted to an early version in your text-editor, using undo and save. 

 
