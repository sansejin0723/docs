---
title: "[Mobile] Verify Element Not Checked" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/mobile-verify-element-not-checked.html 
description: 
---
Description
-----------

Verify if a mobile element is not checked.    

Parameters:  
-------------

Parameter

Parameter Type

Mandatory

Description

to

TestObject 

required

represent a mobile element

timeout 

int

required

system will wait at most timeout (seconds) to return a result

flowControl

FailureHandling

optional

Specify [failure handling](https://docs.katalon.com/x/qAAM) schema to determine whether the execution should be allowed to continue or stop.

Returns
-------

**true** if the element is NOT checked; otherwise, **false**

Example
-------

You want to verify if a checkbox is NOT checked 

Manual: 

** ![](../../images/katalon-studio/docs/mobile-verify-element-not-checked/image2016-8-15 9_56_9.png)**

Script:

```
Mobile.verifyElementNotChecked(findTestObject('SampleApp.apk/android.widget.CheckBox - Checkbox0'), 10)
```