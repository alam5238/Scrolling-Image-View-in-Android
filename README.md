# Scrolling-Image-View-in-Android
Scrolling Image View in Android. Using it like Splash Screen, Games Intro Screen , background moving etc. 

Step::
1. Add Gradle in “build.gradle(Module:app)”.

dependencies {
//scrolling back ground
compile 'com.github.Q42:AndroidScrollingImageView:1.2'
}


2. Check minSdkVersion(requred minimum 17).

3. Add Gradle in “build.gradle(Project:Splashgif)”.

allprojects {
    repositories {
        maven {url 'https://jitpack.io'}
    }
  }
4. Add this line to "AndroidManifest.xml" file for Internet access permission.

<uses-permission android:name="android.permission.INTERNET"/>

5. Add this code to "res/layout/your_activity_name.xml" files.


    <com.q42.android.scrollingimageview.ScrollingImageView
    android:id="@+id/scrollingImageView"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    app:speed=".5dp"
    app:src="@drawable/bg"
    />
    
 6. Copy your Image file and Past it in "res/drawable" folder. 
 7. "app:src="@drawable/bg"" this is linked to image. Here "bg" is the image file. That included in "res/drawable/bg.jpg" . 
 8. Run the Application and Enjoy!! :D 



