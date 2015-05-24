# Setup an Ruboto Android Development Environment

I did all of this on a Oracle VirtualBox VM using various versions of Linux.

## Prerequisits  

1. Download the [Android SDK](http://developer.android.com/sdk/index.html) from the Android Developer Site.
2. Download [Java JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
3. Download [Apache Ant](http://ant.apache.org/)
4. Download [JRuby](http://jruby.org/), or any [Ruby](https://www.ruby-lang.org/en/)
5. If running on Ubuntu 64bit, you'll need the 32bit compiler libraries as well.
  1. http://stackoverflow.com/a/14578798/2009612
  2. http://stackoverflow.com/a/24162990/2009612

## Generic Steps to Setup a Environment

1. Install the Java JDK
  1. Setup the JAVA_HOME environment variable
  2. Setup the $JAVA_HOME/bin in your path
2. Create a ~/android folder, or wherever you want to put it.
  1. This will be called $ANDROID_HOME
3. Unpackage the downloaded sdk files to the $ANDROID_HOME folder
4. place the following folders in the environment for use.
  1. $ANDROID_HOME/tools
  2. $ANDROID_HOME/build-tools
  3. $ANDROID_HOME/platform-tools
5. Extract Apache Ant and place it in your $PATH.
  1. Linux systems, or OS's with a package manager should have this already taken care of.  
6. Use the android tool to download the latest, or desired android versions.
  1. In the terminal, execute the following command: $ android
  2. A GUI will pop up and allow you to download more SDKs, or update existing ones.
7. Create a sample android virtual device, AVD.
  1. When the AVD is finally completely started, install the Ruboto-Core app from the market place.
  2. The AVD will need to have an SD card in order to do this.
  3. If Ruboto-Core is not installed when you attempt to run the application on the AVD, the application will attemtp to install Ruboto-Core from the Play Store. 
8. Install [RVM](https://rvm.io/)
  1. If you're on [Windows](Setup_On_Windows.md), you'll want to use [Pik](https://github.com/vertiginous/pik), or [Uru](https://bitbucket.org/jonforums/uru) to manage your Ruby
9. Install JRuby
10. Make sure to install rake, bundler, and [ruboto](https://github.com/ruboto/ruboto)
11. Create a Ruboto Project
```
ruboto gen app --package org.ruboto.example.quick_start --path quick_start --name quick_start --target android-22 --activity quick_start
```

## Resources

[Resources are listed here.](Resource_Links.md)
