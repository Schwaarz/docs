---
title: "Version 7.x" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/new/version-70.html
redirect_from:
    - "/katalon-studio/new/"
    - "/display/KD/Release+Notes/"
    - "/display/KD/Release%20Notes/"
    - "/katalon-studio/new/all-versions.html"
    - "/katalon-studio/new/version-72.html"
    - "/katalon-studio/new/version-72/"
    - "/katalon-studio/new/version-71/"
    - "/katalon-studio/new/version-71.html"
    - "/katalon-studio/new/version-70/"
description: Release note 7.x
---

## Version 7.2.4

You can download Katalon Studio version 7.2.4 [here](https://github.com/katalon-studio/katalon-studio/releases).

### New Features

* Support editing JVM parameters in Execution Settings. [Learn more](https://docs.katalon.com/katalon-studio/docs/execution-settings.html#execution-settings).

## Version 7.2.3

### Fixes

* Bug: Cannot send SOAP Request due to failure in parsing WSDL definition

## Version 7.2.2

### New Features

- [Web Testing] Support image-based object recognition. [Learn more](https://docs.katalon.com/katalon-studio/docs/manage-web-test-object.html#visual-object-recognition)
- Allow activating Katalon Studio with Katalon TestOps OnPremise Server's licenses

## Version 7.2.0 - 7.2.1

### New Features

* New Windows keywords:
  * [`getElementPosition`](https://docs.katalon.com/katalon-studio/docs/windows-kw-get-element-position.html)
  * [`getElementRect`](https://docs.katalon.com/katalon-studio/docs/windows-kw-get-element-rect.html)
  * [`startApplicationWithTitle`](https://docs.katalon.com/katalon-studio/docs/windows-kw-start-app-title.html)
  * [`switchToWindow`](https://docs.katalon.com/katalon-studio/docs/windows-kw-switch-window.html)
  * [`switchToWindowTitle`](https://docs.katalon.com/katalon-studio/docs/windows-kw-switch-window-title.html)
* New Mobile keywords:
  * [`executeMobileCommand`](https://docs.katalon.com/katalon-studio/docs/mobile-execute-command.html)
  * [`doubleTap`](https://docs.katalon.com/katalon-studio/docs/mobile-double-tap.html)
  * [`longPress`](https://docs.katalon.com/katalon-studio/docs/mobile-long-press.html)
  * [`setEncryptedText`](https://docs.katalon.com/katalon-studio/docs/mobile-set-encrypted-text.html)
* Support adding [Proxy Exceptions](https://docs.katalon.com/katalon-studio/docs/proxy-preferences.html) in Proxy Preferences and `-proxy.excludes` option in console mode.
* [Mobile Recorder] Implement the following actions: Get Text, Swipe, and Scroll To Text.

### Changes and Improvements

* Support ChromeDriver version 79.
* Add **Profiles** to Test Suite Collection Report.
* [Mobile- iOS] Support **Install Dependencies** and **Install WebDriverAgent** tools on the main menu. Please be noted that you have to install [homebrew](https://brew.sh/) manually.
* [Command Syntax] Support both `-serverUrl` and `-serverURL` arguments.
* Make the `DriverFactory.changeWebDriver()` method a public method.
* Support **Open containing folder** for Folders in Test Explorer.

### Fixes

* Bug: [Windows] An issue related to creating a project.
* Bug: An issue related to saving Web Service Message.
* Bug: Empty result tab after a Test Suite execution.
* Bug: Test Script lost parens in method call after editing some steps.
* Bug: [KRE] an issue related to the `retry` option.
* Bug: [Web] Cannot set a timeout in **Wait for options**.
* Bug: [Web Service Request] an issue related to saving HTTP Header.

## Version 7.1.0-7.1.1

### New Features

* Release [Katalon TestOps OnPremise](https://docs.katalon.com/katalon-analytics/docs/ktop-overview.html).
* Support [creating testing licenses](https://docs.katalon.com/katalon-studio/docs/license-management.html#create-and-assign-an-offline-rekse-license) to verify machine ID when creating offline licenses on Katalon TestOps.
* [Katalon TestOps] Support Billing Manager role for being in charge of subscription. [Learn more](https://docs.katalon.com/katalon-analytics/docs/kt-user-role-permission.html).
* Support naming test artifacts, including Test Case, Test Object, Test Data File, Test Suite, Test Suite Collection, and Checkpoint with UTF-8 characters.
* Automatically update keywords' references in other custom keyword classes when renaming or drag-and-dropping a custom keyword.

### Changes and Improvements

* [Web Service] Support all file types of the form-data option in HTTP Body when creating a POST request.
* [Web Service] Support API responses in other languages.
* Auto-healing Smart Xpath becomes a built-in feature of Katalon Studio Enterprise. For standard Katalon Studio users who have already subscribed to this plugin, please contact Katalon team via business@katalon.com.
* Display a progress dialog when adding a bulk number of Test Cases to a Test Suite.
* Handle SVG elements and add a context menu during Spying to capture objects.
* [KRE] Improve running multiple projects with multiple sessions concurrently.
* Support turning off Smart Wait with both global and local settings. [Learn more](https://docs.katalon.com/katalon-studio/docs/webui-smartwait.html).
* [Web Service] Support redirection in POST request and 308 status code.
* Tips: You're recommended to open large HAR files with other tools than Katalon Studio or keep those files not too large for Katalon Studio to read it.

### Fixes

* Bug: Test Suite result is incorrect if a called test case gets failed when *log test steps* is disabled.
* Bug: Web Recorder does not generate XPath locators for SVG elements.
* Bug: [Mobile] Cannot run a browser test on Android device using Appium 1.15.0+.
* Bug: Cannot create a new project when failing to read Sample Projects.
* Bug: Cannot execute test scripts having import paths containing wildcard character (`*`).
* Bug: Cannot start a browser when running with an iOS simulator.
* Bug: NullPointerException when using Katalon Studio for the first time.
* Bug: Cannot read variables in a custom profile if executing a test suite collection remotely.
* Bug: Cannot execute test scripts that have Global Variables' names containing the `$` symbol.
* Bug: An issue related to saving changes in Test Case Variable View.
* Bug: Katalon Studio does not read proxy configuration during Recording.
* Bug: Web Recorder simultaneously generates `NavigateToUrl` keyword and action of an element.

## Version 7.0.0- 7.0.10

### New Features

* Support **Close and Clean up** item in Project menu for closing the project and removing the following items: `.classpath`, and  `.project` files; `bin`, `Libs`, and `.settings` folders.
* Support manually uploading Test Suite Collections' results to Katalon TestOps.
* Support connecting to Git with SSH. [Learn more](https://docs.katalon.com/katalon-studio/docs/git-integration.html)
* Allow configuring the usage tracked by Katalon Studio. [Learn more](https://docs.katalon.com/katalon-studio/docs/katalon-studio-preferences.html).
* Support data-driven testing with additional database sources. [Learn more](https://docs.katalon.com/katalon-studio/docs/database-settings.html).
* Support attaching Katalon Studio's source code for debugging. [Learn more](https://docs.katalon.com/katalon-studio/docs/debugging_test_case.html).
* Support customizing Test Explorer. [Learn more](https://docs.katalon.com/katalon-studio/docs/toolbars-and-views.html#tests-explorer-view).
* Support Test Objects refactoring. [Learn more](https://docs.katalon.com/katalon-studio/docs/test-objects-refactoring.html).
* Support Custom Keywords refactoring. [Learn more](https://docs.katalon.com/katalon-studio/docs/custom-keywords-refactor.html).
* Support private plugins. [Learn more](https://docs.katalon.com/katalon-studio/docs/private-plugins.html).
* Support Windows 10 desktop application testing. See [Windows Desktop Apps Test Design](https://docs.katalon.com/katalon-studio/docs/introduction-desktop-app-testing.html).
* Support sharing test artifacts across projects. [Learn more](https://docs.katalon.com/katalon-studio/docs/import-export-test-artifact.html).
* Support Smart Wait function in a script and a project. See [[WebUI] Smart Wait Function](https://docs.katalon.com/katalon-studio/docs/webui-smartwait.html).
* Support [the WinAppDriver installation](https://docs.katalon.com/katalon-studio/docs/setup-winappdriver.html) and [`Terminate running WebDrivers`](https://docs.katalon.com/katalon-studio/docs/handle-webdrivers.html) options in Katalon Studio Tools.
* Support WebDriver event listeners. [Learn more](https://docs.katalon.com/katalon-studio/docs/webdriver-event-listeners.html).
* Support customizing the Console log. [Learn more](https://docs.katalon.com/katalon-studio/docs/working-with-execution-log.html).
* Support Cucumber keywords executing one or multiple feature files with tags. Learn more about [runFeatureFileWithTags](https://docs.katalon.com/katalon-studio/docs/cucumber-kw-run-feature-file-tag.html) and [runFeatureFolderWithTags](https://docs.katalon.com/katalon-studio/docs/cucumber-kw-run-feature-folder-tag.html).

### Changes and Improvements

* [Web Service] Encode special characters in query parameters.
* Revert **IEDriverServer** from 3.141.59 to 3.6.0.
* [Console mode] The `katalon` launcher is replaced by `katalonc` and there is a separate app named **Katalon Studio Runtime Engine** for executing Katalon Studio in console mode. Click [here](https://www.katalon.com/download/) to download.
* Convert **qTest** and **Kobiton** built-in integrations into plugins.
* Display errors of test scripts in the **Problems** view.
* Support ChromeDriver version 77 and IEDriverServer version 3.141.59.
* Show a full stack trace of an exception thrown by custom classes in Test Hooks.
* Support manually uploading test suite collections' results to Katalon TestOps.
* [Web Service] Support passing proxy details through the script. [Learn more](https://docs.katalon.com/katalon-studio/docs/proxy-preferences.html#pass-proxy-details-through-the-script).
* Update documents of [Katalon Studio API Specification](https://docs.katalon.com/javadoc/index.html) to version 7.0.0.
* Upgrade Apache POI to version 3.17.
* Dynamic Querying Test Suite is renamed Dynamic Test Suite.
* Add plugins reloading options to the Project Settings.
* Support parsing the Request Message's template from the associated `XSD` file when importing test objects from WSDL.
* Support adding the Organisation ID parameter to the Command Generator.
* Support selecting a Katalon TestOps's organization on the activation.
* Enhancement: Add some JVM options to reduce Katalon Studio's memory consumption.
* Support a hotkey of Spy Utility in Web Recorder to capture objects. [Learn more](https://docs.katalon.com/katalon-studio/docs/record-web-utility.html).
* Update **Quick Start** in Katalon Studio after activation.
* Support adding `.gitignore` and `build.gradle` files when creating a project.
* Support uploading reports with pdf, HTML, CSV formats (generated by Basic Report plugin) to Katalon TestOps. [Learn more](https://docs.katalon.com/katalon-studio/docs/katalon-analytics-beta-integration.html).
* Support submitting test run results with captured videos to Katalon TestOps. [Learn more](https://docs.katalon.com/katalon-studio/docs/katalon-analytics-beta-integration.html).
* Support uploading the `*.rp` file to Katalon TestOps to parse more information on test results.
* Support creating a test plan right from the test suite collection screen in Katalon Studio to enhance the integration of Katalon Studio with Katalon TestOps. [Learn more](https://docs.katalon.com/katalon-studio/docs/katalon-analytics-beta-integration.html).
* Support uploading Project Code from Katalon Studio to Katalon TestOps. [Learn more](https://docs.katalon.com/katalon-studio/docs/katalon-analytics-beta-integration.html).
* Update the integration mechanism with Katalon TestOps. [Learn more](https://docs.katalon.com/katalon-studio/docs/katalon-analytics-beta-integration.html).
* Update the integration configurations with Katalon TestOps when a new project is created.
* Support auto-filling the input of [Katalon API Key](https://docs.katalon.com/katalon-studio/docs/katalon-apikey-70.html) in the command-line generator.
* Support generating test results in JUnit format.
* Support uploading reports of test suite collections to Katalon TestOps.
* Remove unnecessary information in the console log when users execute in the console mode for the first time.
* Support passing more information to the console mode execution with `--info -buildLabel="text" -buildURL="text"`. See [General Options ](https://docs.katalon.com/katalon-studio/docs/console-mode-execution.html#general-options) in Console Mode Execution.
* Upgrade the activation mechanism in Katalon Studio to seamlessly integrate with Katalon TestOps. See [Activate Katalon Studio](https://docs.katalon.com/katalon-studio/docs/katalon-studio-activation-since-70.html).
* Merge the Plugins menu into the Tools menu.
* Support MySQL Database version **8.0.17**.
* Support automatically reloading plugins when opening a project.

### Fixes

* Bug: [DDT] Cannot get values from data files with database type in a test case.
* Bug: Cannot log in to Katalon Studio with passwords containing special characters.
* Bug: [Web Service] SOAP response has an empty header.
* Bug: Cannot reload plugins with credentials containing special characters.
* Bug: The **Results** tab of Test Suites/Test Suite Collection fails to automatically refresh after the first execution.
* Bug: **Show references** of test objects fails to display the objects' references in global variables and test case variables.
* Bug: Cannot send SOAP requests when **WSDL** files contain the relative `xsi:schemaLocation`.
* Bug: [WebUI Keyword] The `WebUI.clickImage` keyword fails to perform.
* Bug: [Web Service] `getCurrentRequest()` always gets default values instead of a variable's values passed from test case.
* Bug: Incorrectly return code when **Follow redirects** is disabled in Web Service Request. [More details](https://forum.katalon.com/t/followreridects-does-not-work/33800).
* Bug: Cannot save modifications in the configuration tab of the Web Service Request.
* Bug: Cannot detect mobile test objects having parameterized global variables in their properties.
* Bug: [Console Mode] To retry executing failed test cases in Test Suite Collection fails to return the correct exit code.
* Bug: [Data Binding] An issue causes binding Variables to Test Data to fail.
* Bug: [WebService] Verification Editor doesn't keep Unicode characters.
* Bug: [Mobile Testing] Cannot retry executing failed test cases.
* Bug: Web service response displays garbled text as non-Latin characters.
* Bug: [Basic Report Plugin] CSV Report status is always Incomplete.
* Bug: The Log Viewer’s cursor incorrectly renders when selecting a log message.
* Bug: Newly added variables disappear after a switch from the Variable tab to another tab.
* Bug: An issue related to Variable binding when the data contains special characters.
* Bug: The Delay keyword doesn't work when the passing data is BigDecimal.
* Bug: Har files disappear after having been opened for the first time with the current Web Service object.
* Bug: [Custom Keyword] an issue related to the default package name when users create a keyword without entering a package name.
* Bug: [Katalon TestOps] Cannot navigate to the URL configured by users in View Execution History.
* Bug: [Katalon TestOps] an issue related to the error message when users create a new project for the invited team without permission.
* Bug: [GlobalVariable] Cannot execute a script with a profile that has a Global Variable with invalid syntax.
* Bug: [WebUI Keywords]  The `verifyElementPresent()` and `verifyElementNotPresent()` keywords should return `false` instead of throwing an exception when the verified elements do not exist.
* Bug: The `Delay between actions` fails to perform as configured.
* Bug: An issue causes `callTestCase` to fail.
* Bug: `findWebElements` fails when the `Default wait for element timeout` is set to 0 in the Execution Settings.
* Bug: [Web Recorder] An issue related to the `Cannot save entity: file path length limit exceeded.` error when saving test objects.
* Bug: Custom Keywords are not displayed in the Recent keywords after being used.
* Bug: An issue related to renaming a folder with uppercase or lowercase characters. [More details](https://github.com/katalon-studio/katalon-studio/issues/189).
