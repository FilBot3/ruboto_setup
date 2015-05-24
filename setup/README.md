# Setup an Ruboto Android Development Environment

## Prerequisits  

1. Download the Android SDK from the Android Developer Site.
2. Download Java JDK
3. Download Apache Ant
4. Download JRuby, or any Ruby

## Steps to Setup the Environment

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
6. use the android tool to download the latest, or desired android versions.
7. Create a sample android virtual device, AVD.
8. Install RVM
9. Install JRuby
10. Make sure to install rake, bundler, and ruboto
11. Attempt to create a Ruboto Project

## Resources

1. http://www.ibm.com/developerworks/library/wa-ruby/
2. http://developer.android.com/sdk/index.html#Other
3. https://github.com/ruboto/ruboto/blob/master/README.md
4. https://github.com/ruboto/ruboto/wiki/Setting-Up-a-Ruboto-Development-Environment
5. https://github.com/ruboto/ruboto/wiki/Environment-setup-for-ubuntu
6. https://github.com/ruboto/ruboto/wiki/Environment-setup-for-windows
