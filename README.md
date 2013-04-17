# iconpack_template

Eclipse Iconpack Project

Works with Go-, Holo(HD)-, ADW-, Nova- and Apex-Launcher


## Instructions

### Api
Make sure you have API 8 installed!

	Window -> Android SDK Manager -> Check Android 2.2 (API 8) -> Install packages

### Installation
Get the project either by cloning the repository or downloading it as a zip/tar.gz file.

Then when you have it unpacked in a location of your choosing you can open a new project in Eclipse and create a new Android project from existing code.


#### Step 1
Update source package in `MainActivity.java` and `AndroidManifest.xml`.

In `AndroidManifest.xml` you should update this `package="com.yourname.appname"` to something that matches your icon pack, i.e. `com.brownbear.foresticons`.

Go to src and right click on the package `com.yourname.appname`, choose Refactor, Rename and enter the same domain you did in the `AndroidManifest.xml`.


#### Step 2
Update version information in `AndroidManifest.xml` before each release to Google Play Store.

	android:versionCode="1"
Increment +1 with every upload to GooglePlayStore

	android:versionName="1"
Whatever you want, can be "abc" or "1.2.3.4"


#### Step 3
It should be self-explanatory what to change in `res/values/strings.xml`


#### Step 4
Copy your icons to `res/drawable-hdpi`.
Name them according to the icon names in `drawable.xml` and `appfilter.xml` or rename in the xml-files to match your icons.


#### Step 5
Once you create an apk with this template just update the following files which are identical but in different places to work with different launchers.

appfilter.xml
	/MainActivity/res/xml/appfilter.xml
	/MainActivity/assets/appfilter.xml

drawable.xml
	/MainActivity/res/xml/drawable.xml
	/MainActivity/assets/drawable.xml

icon_pack.xml
	/MainActivity/res/values/icon_pack.xml
	/MainActivity/assets/icon_pack.xml

## License
The MIT License (MIT) Copyright (c) 2013 Ricard Aspeljung

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
