---
title: "[WebUI] Verify Image Present" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/webui-verify-image-present.html 
description: 
---
Description 
------------

Verify if an image is present on page.

Parameters 
-----------

Param

Param Type

Mandatory

Description

to

TestObject

Required

Represent an image.

flowControl

FailureHandling

Optional

Specify [failure handling](https://docs.katalon.com/x/qAAM) schema to determine whether the execution should be allowed to continue or stop.

Returns 
--------

Param Type

Description

Boolean

*   true if the image if present.
    
*   false if the image is not present.
    

Example 
--------

You want to verify if "img_KatalonLogo" is present on page.

```
import static com.kms.katalon.core.checkpoint.CheckpointFactory.findCheckpoint
import static com.kms.katalon.core.testcase.TestCaseFactory.findTestCase
import static com.kms.katalon.core.testdata.TestDataFactory.findTestData
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject
import com.kms.katalon.core.checkpoint.Checkpoint as Checkpoint
import com.kms.katalon.core.checkpoint.CheckpointFactory as CheckpointFactory
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as MobileBuiltInKeywords
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as Mobile
import com.kms.katalon.core.model.FailureHandling as FailureHandling
import com.kms.katalon.core.testcase.TestCase as TestCase
import com.kms.katalon.core.testcase.TestCaseFactory as TestCaseFactory
import com.kms.katalon.core.testdata.TestData as TestData
import com.kms.katalon.core.testdata.TestDataFactory as TestDataFactory
import com.kms.katalon.core.testobject.ObjectRepository as ObjectRepository
import com.kms.katalon.core.testobject.TestObject as TestObject
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WSBuiltInKeywords
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WS
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUiBuiltInKeywords
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI
import internal.GlobalVariable as GlobalVariable

'Open browser and navigate to a site that contains an image'
WebUI.openBrowser(GlobalVariable.G_SiteURL)

'Verify if the image is present'
WebUI.verifyImagePresent(findTestObject('img_KatalonLogo'))

'Close browser'
WebUI.closeBrowser()


```

The test object needs to define a source image from the local machine for Katalon Studio to use it for verification

![](../../images/katalon-studio/docs/webui-verify-image-present/define_image.jpg)