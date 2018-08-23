---
title: "Update or Replace Web Browser Drivers and Selenium" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/update-or-replace-web-browser-drivers-and-selenium.html 
description: 
---
For manually replacing and updating other versions of WebDrivers and Selenium, please refer to this [guide](https://docs.katalon.com/x/1xtO). 

Katalon Studio team strongly suggest users **NOT** to manually replace or update any WebDrivers. Any changes in drivers may cause runtime bugs for Katalon Studio application.

Katalon Studio V5.1.0

How to Replace 

 

**Windows**

**MAC OSX**

Selenium [3.7.1](https://raw.githubusercontent.com/SeleniumHQ/selenium/master/java/CHANGELOG)

*   **Download** the desired Selenium version [here](http://selenium-release.storage.googleapis.com/index.html) (Select **only** Selenium 3.0+ and higher version than 3.7.1)
*   **Delete** existing selenium-server-standalone-3.x.jar  
    
*   **Copy** preferred **driver** into this folder  
    <Katalon Studio folder>\\configuration\\resources\\lib

*    /Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/lib

Chromedriver [2.33](https://chromedriver.storage.googleapis.com/2.33/notes.txt)

*   **Download** preferred Chromedriver [here](https://sites.google.com/a/chromium.org/chromedriver/downloads)
*   **Copy** downloaded Chromedriver and **paste** into Katalon Studio folder

You can use 32-bit Windows Chromedriver for both 32-bit and 64-bit Windows.

*   *   <Katalon Studiofolder>\\configuration\\resources\\drivers\\chromedriver_win32
    *   <Katalon Studiofolder>\\configuration\\resources\\drivers\\chromedriver_win64

*   /Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/drivers/chromedriver_mac

Firefox (Gecko Driver) [0.19](https://github.com/mozilla/geckodriver/releases/tag/v0.19.0)

*   **Download** preferred Gecko Driver [here](https://github.com/mozilla/geckodriver/releases)
*   **Copy** downloaded Gecko driver and **paste** into Katalon Studio folder
    *   <Katalon Studio folder>\\configuration\\resources\\drivers\\firefox_win32
    *   <Katalon Studio folder>\\configuration\\resources\\drivers\\firefox_win64

*   /Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/drivers/firefox_mac

IEDriverServer [3.6.0](https://raw.githubusercontent.com/SeleniumHQ/selenium/master/cpp/iedriverserver/CHANGELOG)

*   Download preferred IEDriver [here](http://selenium-release.storage.googleapis.com/index.html)
*   **Copy** downloaded IEDriverServer and **paste** into Katalon Studio folder
*   <Katalon Studio folder>\\configuration\\resources\\drivers\\iedriver_win32
*   <Katalon Studio folder>\\configuration\\resources\\drivers\\iedriver_win64