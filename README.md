# Away Builder

This is a custom fork kept in sync with ![away3d](https://github.com/ZeroIPDev/away3d). New features include:
- Sprite3D support: Add key-pair `Sprite3D`:`Material name` on ObjectContainer3D (context menu option available)

## Install SDKs
1. Download ![Apache Flex SDK](https://flex.apache.org/download-binaries.html) and extract to your preferred location
2. Download Adobe AIR SDK ([Windows](https://airdownload.adobe.com/air/win/download/32.0/AdobeAIRSDK.zip)/[Mac](https://airdownload.adobe.com/air/mac/download/32.0/AdobeAIRSDK.dmg)) and extract into the same directory as the Flex SDK, overwriting files if necessary
3. Copy `env-template.properties` in your SDK folder as `env.properties`
4. Uncomment `env.AIR_HOME` and point it to the full path of your SDK

## How to build
1. Run `git clone https://github.com/Fancy2209/away3d-core-fp11 -b dev` inside this repo
2. Install the VSCode Extension "AS3 & MXML" by Bowler Hat
3. Open the repo in VSCode
4. Point VSCode to to the SDK you setup during installation
5. Press **CTRL + Shift + P** and run the command "ActionScript: Quick Compile and Debug (Experimental)" to debug, or use the builds tasks in the **CTRL + Shift + B** shortcut to assemble a release build

Flex SDK: 4.9.1+  
AIR SDK: 3.7+  
use _"-swf-version 20"_

## awaybuilder-core
Flex library project that contains shared sources for all Away Builder applications.  
Project type: Flex library for desktop  

### Project file structure:
_src/_ - main source directory  
_libs/_ - library directory with .swc files.

### Files to include in the library:
* __src/assets/*__  
* __src/defaults.css__  

## awaybuilder-desktop
Project must be set up as Flex AIR project  

### Project file structure:
_src/_ - main source directory  
_src/AwayBuilderApplication.mxml_ - main application  
_src/AwayBuilderApplication-app.xml_ - AIR application descriptor  

_awaybuilder-core_ project must be added as linked library  
