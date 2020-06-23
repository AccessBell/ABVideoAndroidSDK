# ABVideoAndroidSDK
Android SDK for AccessBell video conferencing

The following is a guide on how to set up the sdk in an existing Android project.

Add the Maven repository in the build.gradle file for the Android Studio application.

        allprojects {
            repositories {
                google()
                jcenter()
                maven {
                    url "https://github.com/accessbell/ABVideoAndroidSDK/raw/master/releases"
                }
            }
        }

Add the following implementation under the dependencies section of the build.gradle section.

    implementation ('org.accessbell.react:accessbell-meet-sdk:2.9.0') { transitive = true }
    
Rebuild your application and use the sdk by adding "import org.accessbell.meet.sdk" to the respective files in which you want to
display your video conference.
