#Build it Bigger(Gradle for Android and Java Final Project)

##Overview

 This app is created for multiple flavors(free/paid) that uses multiple libraries and Google Clould Endpoints. The finished app will consist of four modules :
 
 (i) A Java library that provides jokes,  

 (ii) a **Google Clould Endpoints (GCE)** project that serves those jokes, 

 (iii) an Android Library containing an activity for displaying jokes, 
 
 (iv) and an Android app that fetches jokes from the GCE module and passes them to the Android Library for display
  
This app helped me to learn how to
 
* Add free and paid flavors to an app, and set up your build to share code between them
 * Factor reusable functionality into a Java library
 * Factor reusable Android functionality into an Android library
 * Configure a multi project build to compile your libraries and app
 * Use the Gradle App Engine plugin to deploy a backend
 * Configure an integration test suite that runs against the local App Engine development server


![ezgif com-resize](https://cloud.githubusercontent.com/assets/15085932/14649300/fa5cb090-0683-11e6-8daf-286e05bc5ffa.gif)    
**Free Version with ads**

![ezgif com-resize 1](https://cloud.githubusercontent.com/assets/15085932/14649517/158290c8-0685-11e6-8f2f-cf4353e8223a.gif)

**Paid version without ads**

##Prerequisites

* The app is built with compileSdkVersion 23 and requires [JDK 7](http://oracle.com/technetwork/java/javase/downloads/index.html) or higher
 
* Android Studio

The app source code is provided in the course [repository](https://github.com/udacity/ud867/tree/master/FinalProject). It contains an activity with a banner ad and a button that purports to tell a joke, but actually just complains. The banner ad was set up following the instructions [here](:https://developers.google.com/mobile-ads-sdk/docs/admob/android/quick-start)

You may need to download the Google Repository from the Extras section of the Android SDK Manager

###Implementation Steps###

Refer [wiki](https://github.com/Ruchita7/Build_it_bigger/wiki/Implementation-steps)


##Instructions

###Get the source codes

Get the source code of the library and example app, by cloning git repository or downloading archives.

 * If you use **git**, execute the following command in your workspace directory.
 
    `$ git clone https://github.com/Ruchita7/Build_it_bigger.git`
    
* If you are using Windows, try it on GitBash or Cygwin or something that supports git.
 
###Import the project to Android Studio
 
Once the project is cloned to disk you can import into Android Studio:

 * From the toolbar select **File > Import Project**, or Import Non-Android Studio project from the Welcome Quick Start.

 *  Select the directory that is cloned. If you can't see your cloned directory, click "Refresh" icon and find it.

 *  Android Studio will import the project and build it. This might take minutes to complete. Even when the project window is opened, wait until the Gradle tasks are finished and indexed.

 *  Connect your devices to your machine and select app from the select Run/Debug Configuration drop down.Click the Run button

###Build and install using Gradle

If you just want to install the app to your device, you don't have to import project to Android Studio.

 •  After cloning the project, make sure **ANDROID_HOME** environment variable is set to point to your Android SDK. See [Getting Started with Gradle](https://guides.codepath.com/android/Getting-Started-with-Gradle).

 •  Connect an Android device to your computer or start an Android emulator.

 •  Compile the sample and install it. Run gradlew installDebug. Or if you on a Windows computer, use **gradlew.bat** instead.
 
###Contributing

Please follow the **"fork-and-pull"** Git workflow while contributing to this project

 **Fork** the repo on GitHub

 **Commit** changes to a branch in your fork

 **Pull request "upstream"** with your changes

 **Merge** changes in to "upstream" repo

**NOTE:** Be sure to merge the latest from **"upstream"** before making a pull request!
 
###FAQs

**The project can no longer be compiled/imported if I move it to another directory**

I typically include the dependencies in the repo and have them already linked, so if you move the project you'll need to also update the path to the dependency. To do this, modify the project.properties file of the project

**I'm getting an error saying that there are multiple versions of a jar**

To fix this, make sure that all the jars you are using conform to the same version. You can do this by just replacing all the problematic jars with the version you would like to use.
 

