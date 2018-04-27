# CordovaUnityIntegration

Download and extract files from here - https://george.dbpx.co/empty.zip

"empty" folder (put on desktop) - the cordova project - the Xcode project is under platforms/iOS folder

"EmptyUnity" folder (put on desktop) - the Unity project

https://github.com/yasirkula/UnityIonicIntegration - download as zip and unzip it. Leave the resulted folder in Downloads 

From there I only think the UNITY_IOS_EXPORTED_PATH variable needs to change to the absolute path of the Unity export.

Also, make sure you change the code signing to your own one.

So if you follow the folder placement you will only need to change the username in that that route.

/Users/DBS/Deskop/EmptyUnity/build1/ becomes /Users/%YOURUSERNAME%/Desktop/EmptyUnity/build1/

Then you can follow the instructions below to reproduce the errror.
 
Connect Device 

Open the project from the the platforms/ios 

Make sure all the build schemes are set on build and the debug executable is checked. 

Run on device as release. 

Hard close app. 

Open safari and navigate to "empty://" to simulate opening tap once when the deviceready has fired

That's where the app crashes when opening from the App Store/ other apps.
