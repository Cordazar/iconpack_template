Eclipse Iconpack Project

Make sure you have API 8 installed!
Window -> Android SDK Manager -> Check Android 2.2 (API 8) -> Install packages

File -> Import -> Android -> Existing Android.... -> OK

First you have to change the following points:

#1 
MainActivity/src/com.yourname.appname -> Right click -> Refactor -> Rename -> Enter something like com.WHATEVER.WHATEVER -> ok

#2
MainActivity/AndroidManifest.xml
[...]
package="com.yourname.appname" <- com.WHATEVER.WHATEVER (see above)
android:versionCode="1" <- +1 with every upload in GooglePlayStore
android:versionName="1" <- Whatever you want, can be "abc" or "1.2.3.4"

#3
It should be self-explanatory what to change in
/MainActivity/res/values/strings.xml


#4
Copy your icons to MainActivity/res/drawable-hdpi 

#5 
Once you create an apk with this template just update the following files

#Both these files are identical
/MainActivity/res/xml/appfilter.xml
/MainActivity/assets/appfilter.xml

#Both these files are identical
/MainActivity/res/xml/drawable.xml
/MainActivity/assets/drawable.xml

#Both these files are identical
/MainActivity/res/values/icon_pack.xml
/MainActivity/assets/icon_pack.xml


If you have any questions, ideas how to improve this project, or you want to collaborate email me gmaedzl@playstore.com
