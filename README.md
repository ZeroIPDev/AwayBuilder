# Away Builder

# How to build
1. Follow this guide to install the [Apache Flex SDK with AIR](https://joshblog.net/2024/how-to-install-apache-flex-with-adobe-air-from-harman/)
2. Run `git clone https://github.com/Away3D/away3d-core-fp11 -b dev` inside this repo
3. Install the VSCode Extension "AS3 & MXML" by Bowler Hat
4. Open the repo in VSCode
5. Point VSCode to to the SDK you setup in Step 1
6. Press CTRL + P and run the command "ActionScript: Quick Compile and Debug (Experimental)"

Flex SDK: 4.9.1  
AIR SDK: 3.7  
use _"-swf-version 20"_  
latest away3d-core: _https://github.com/away3d/away3d-core-fp11/tree/dev_  

## awaybuilder-core
Flex library project that contains shared sources for all Away Builder applications.  
Project type: Flex library for desktop  

### Project file structure:
_src/_ - main source directory  
_libs/_ - library directory with .swc files.

### Files to include in the library:
* __src/assets/*__  
* __src/defaults.css__  

(in Flash Builder: Project Properties -> Flex Library Build Path -> Assets -> select All)

## awaybuilder-desktop
Project must be set up as Flex AIR project  

### Project file structure:
_src/_ - main source directory  
_src/AwayBuilderApplication.mxml_ - main application  
_src/AwayBuilderApplication-app.xml_ - AIR application descriptor  

_awaybuilder-core_ project must be added as linked library  
