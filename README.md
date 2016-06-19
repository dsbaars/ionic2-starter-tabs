Ionic 2 Tabs Starter
====================

To use this as ionic v2 starting project:

0. create `ionic.config.json`, `package.json`, `config.xml`
0. (optional) create `gulpfile.js`

#### ionic.config.json
````json
{
  "name": "<appname>",
  "app_id": "",
  "v2": true
}
````

#### package.json
````json
{
  "dependencies": {
    "@angular/common": "^2.0.0-rc.1",
    "@angular/compiler": "^2.0.0-rc.1",
    "@angular/core": "^2.0.0-rc.1",
    "@angular/http": "^2.0.0-rc.1",
    "@angular/platform-browser": "^2.0.0-rc.1",
    "@angular/platform-browser-dynamic": "^2.0.0-rc.1",
    "@angular/router": "^2.0.0-rc.1",
    "es6-shim": "^0.35.0",
    "ionic-angular": "2.0.0-beta.9",
    "ionic-native": "1.2.4",
    "ionicons": "3.0.0",
    "reflect-metadata": "^0.1.3",
    "rxjs": "5.0.0-beta.6",
    "zone.js": "^0.6.12"
  },
  "devDependencies": {
    "del": "2.2.0",
    "gulp": "3.9.1",
    "gulp-watch": "4.3.5",
    "ionic-gulp-browserify-typescript": "^1.1.0",
    "ionic-gulp-fonts-copy": "^1.0.0",
    "ionic-gulp-html-copy": "^1.0.0",
    "ionic-gulp-sass-build": "^1.0.0",
    "ionic-gulp-scripts-copy": "^2.0.0",
    "run-sequence": "1.1.5"
  },
  "cordovaPlugins": [
    "cordova-plugin-device",
    "cordova-plugin-console",
    "cordova-plugin-whitelist",
    "cordova-plugin-splashscreen",
    "cordova-plugin-statusbar",
    "ionic-plugin-keyboard"
  ],
  "cordovaPlatforms": [
    "ios",
    {
      "platform": "ios",
      "version": "",
      "locator": "ios"
    }
  ]
}
````

config.xml
````xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<widget id="com.ionicframework.appname" version="0.0.1" xmlns="http://www.w3.org/ns/widgets" xmlns:cdv="http://cordova.apache.org/ns/1.0">
  <name>ionic-appname</name>
  <description>An Ionic Framework and Cordova project.</description>
  <author email="hi@ionicframework" href="http://ionicframework.com/">Ionic Framework Team</author>
  <content src="index.html"/>
  <access origin="*"/>
  <allow-intent href="http://*/*"/>
  <allow-intent href="https://*/*"/>
  <allow-intent href="tel:*"/>
  <allow-intent href="sms:*"/>
  <allow-intent href="mailto:*"/>
  <allow-intent href="geo:*"/>
  <platform name="android">
    <allow-intent href="market:*"/>
  </platform>
  <platform name="ios">
    <allow-intent href="itms:*"/>
    <allow-intent href="itms-apps:*"/>
  </platform>
  <preference name="webviewbounce" value="false"/>
  <preference name="UIWebViewBounce" value="false"/>
  <preference name="DisallowOverscroll" value="true"/>
  <preference name="android-minSdkVersion" value="16"/>
  <preference name="BackupWebStorage" value="none"/>
  <preference name="SplashScreenDelay" value="2000"/>
  <preference name="FadeSplashScreenDuration" value="2000"/>
  <feature name="StatusBar">
    <param name="ios-package" onload="true" value="CDVStatusBar"/>
  </feature>
  <plugin name="cordova-plugin-device" spec="~1.1.2"/>
  <plugin name="cordova-plugin-console" spec="~1.0.3"/>
  <plugin name="cordova-plugin-whitelist" spec="~1.2.2"/>
  <plugin name="cordova-plugin-splashscreen" spec="~3.2.2"/>
  <plugin name="cordova-plugin-statusbar" spec="~2.1.3"/>
  <plugin name="ionic-plugin-keyboard" spec="~2.2.0"/>
</widget>
````
