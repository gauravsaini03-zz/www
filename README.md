cordova-communityapp
====================

Mifos Community App in Cordova

App Build Instructions

Download Android

* Download sdk from this url https://developer.android.com/sdk/index.html
* Unzip the folder in your home directory
* Edit the bashrc  file and add below lines (bashrc file is hidden file in linux in home directory )
<pre>
PATH DEFAULT=${PATH}:/path/to/tools
PATH DEFAULT=${PATH}:/path/to/platform-tools
ANDROID_SDK_HOME=/path/to/tools
</pre>

Install nodejs and cordova

<pre>
sudo apt-get install npm
sudo npm install -g cordova
</pre>

Checkout www into you application. (replacing with default)

<pre>
cordova create communityapp
cd communityapp
rm -r www/
git clone https://github.com/gauravsaini03/www.git
cordova platform add android
cordova run android
</pre>
