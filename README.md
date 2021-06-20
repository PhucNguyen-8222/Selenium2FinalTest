# TADashboard--PhucTeam
# SELENIUM 2 -- AUTOMATION FRAMEWORK

A test framework for Selenium 2 automation

## What should you have before starting

Windows
* [IntelliJ Community/Ultimate edition](https://www.jetbrains.com/idea/download/#section=windows) (recommended, you can use other IDEs but may have to install additional plugins for it to work and this guide is only focused on IntelliJ)
* [Maven](https://maven.apache.org/install.html)
* [JDK 8](https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html)
* Create a new SDK in IntelliJ linked to this Virtual environment
* Link your IntelliJ project to this SDK.



## Setting up the project
1. Download the source code in [here](https://github.com/SeleniumLV2-2021/TADashboard--PhucTeam)
2. Start IntelliJ, ```File``` -> ```Open``` -> ```TADashboard``` and choose ```pom.xml```
3. Continue select ```SeleniumCore``` and choose ```pom.xml```   
4. Open ```Maven``` and wait for dependencies to be installed

## Framework
Since the framework was designed with Selenium Core exercises, it began with just that. However, it has been extended to do several other things and test components of others.

### 1. **How to create a new Suite**
**To create testNG XML file for running the Suite, follow with steps:**
* Step 1: Go to ```TADashboard``` -> ```src``` -> ```test``` -> ```resource```
* Step 2: Right click on ```resource``` -> select ```New``` -> select ```File```.
* Step 3: Create a ```testNG.xml``` file and click on ```Finish``` button.
* Step 4: Write the first TestNG XML to run TestNG test suites.
* Example for TestNG XML file 
```
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd">
<suite name="PreTest" thread-count="1" parallel="tests">
    <test name="ChromeTest">
        <parameter name="browser" value="chrome.local"/>
        <classes>
            <class name="com.test.Test.LoginTest"/>
        </classes>
    </test>
</suite>
```
**Note**
* < suite > The suite tag can be given any name and denotes the test suite name.
* < test > The test tag can be given any name and indicates your test sets.
* < classes > This is the combination of your package name and test case name and cannot write anything else. >
### 2. **How to run a test**
**Have 2 options to run a test**
* Option 1: Click on the ```testNG.xml``` file and select ```Run```
* Option 2: Go to the test file want to test and run each test case
## License

✨✨ Group 1 ✨✨
