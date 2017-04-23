# Pain of building React-Native

## So I am a Linux fan and completely in love with Ubuntu (currently running 16.04)

## In my development practice I have never felt such struggle and pain configuring any of the frameworks or api or any 3rd party library.. Talking about React-Native.. I don't know why but it was really tough for me just to run the basic "hello world" code of this framework.. Don't know surely how others feel for the first time configuring this framework but I had a really painful experinece to be honest.

## The very first step was to follow the guideline here:
https://facebook.github.io/react-native/docs/getting-started.html

## Installed and configured each and everything without the watchman and flow. Installing android studio and the packages were too much sensitive and also setting up the environment for the android sdk,tools etc.
 
## AVD (Android Virtual Device) was the real pain.. Still couldn't be able to connect and get the output on my real device properly..

## Installed the react-native cli and created the app perfectly.. But the problem was when the project were fired to be build.. Too much error I have faced in this specific session.. The major problems were:

	1. AVD configure.. Couldn't create a virtual device for the first time.

	2. Tried with CRNA, that went well because of Expo App.. I was trying to solve the official doc problems side by side but no progress.. There were one problem after another in a very long loop..

	3. Decided to stick with CRNA, I felt totally fade up with the main react-native building errors. I was followed starting the official tutorial and faced problem again.. Don't know the specific reasons but there were errors found in the official react native tutorial and doc code.. And there were some little differences with the code structure between the official doc codes and CRNA codes.

	4. Decided to go back again with the main react-native build. Errors after Error. Some major problems found in the android/build.gradle file.. the "dependencies-classpath" defining (means editing) and defining the sdk and adb.. Though I havn't still found the right way to define adb.. This may be the reason why I can't use my real android device..

	5. Also I had to create local.properties file defining the environment variables (sdk,adb etc)

	6. And Android/graddle/wrapper/graddle-wrapper.properties edited was a self invention.. Graddle was needed to changed to the latest version.. (hope that encountered the ".javac" error..

	7. And the last project which was built with success, before that while I was trying to build another project, when some error occured, I found a solution through google like this: in the build.gradle file the buildscript-repositories needed one edit in the section: "" jcenter { url "http://jcenter.bintray.com/" } "".. Though that project was not build properly for some reason.. Updating the graddle to the latest as I mention on no. 6 helped me to get through all of these suffurings..

## After the successful build I tried to convert the react-native app to an Expo project.. That is not properly working.. Also tried to build react-native android from source.. same not satisfactory result..

## So now the target is to be familiar with the tutorials and the official docs..


