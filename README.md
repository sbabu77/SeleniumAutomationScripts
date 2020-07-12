# SeleniumAutomationScripts
Selenium Automation Scripts Code

Testing and Automation Language –  
AUTOMATION - Any process or procedure performed with MINIMAL human intervention. 
MINIMAL does not mean zero - sometimes all human intervention too difficult to remove. Automation focuses on minimizing human procedures, not eliminating them. 
Automation is considered TOUCHLESS when it can run entirely without human intervention. We consider all test cases in our existing functional regression automation suite to be TOUCHLESS because they run to completion once triggered. 
 
An Automation test scenario is considered complete when it has been committed to GitHub, and can be run on a “non-local” machine. For UI scenarios, this means on the Selenium grid VDI’s. For non-UI, this means from a user’s machine that did not write the test case. 
 
All below forms of testing can be performed in a MANUAL OR AUTOMATED fashion.
 
Types of testing:
•         Service Testing - Testing that calls on a web service or a group of web services, and validates the text response (XML or JSON). This is performed using tools (ex. SOAPUI) or libraries (ex. REST Assured). 
•         UI Testing - Testing that is directly interacting with the front end user interface (clicking on buttons, typing into text boxes), and validates expected behavior (error message is displayed). This is performed using tools (ex. UFT), or libraries (ex. Selenium). 
 
Classes of testing:
•         Unit Testing – Testing of a new requirement at the code level (typically performed by developers).
•         Functional Testing – Testing of SPECIFIC requirements above the code level (as defined by a user story or requirements document). Functional Tests should fail until the expected feature is implemented. 
•         Regression Testing – Testing of overall application integrity following FUNCTIONAL testing. Regression tests should always pass, failure should indicate the presence of a defect. 
•         End to End Testing – Testing of an entire application flow (Claim Creation to Payment). 
 
•         Smoke Testing - A shortlist of test scenarios that cover the critical business functionality of the application. These are to be run after EVERY build of the application to verify that the core functionality has not been impacted. 
 
•         Integration Testing - Testing of two distinct units of an application.
•         Interface Testing - Testing the communication between two different software systems.
 
Important consequences of the above:
REGRESSION test cases are FUNCTIONAL test cases.
INTERFACE test cases are also considered REGRESSION test cases, but are NOT considered FUNCTIONAL test cases. 
 
REGRESSION encompasses ALL testing that is performed by Systems team before a release. 
Testing of the core ECOS, FNOL, Portal applications is called FUNCTIONAL REGRESSION.
Testing of the communication between ECOS and other systems (RAD, CCPS) is called INTERFACE REGRESSION.

What’s automated?
In Agile, Functional Testing happens within scrum teams in the sprint itself. Automation maturity varies by team. 
Functional Regression Testing is all automated, and covers 42% of all requirements, and 80% of critical and high requirements. All functional regression testing today is UI, with the exception of work in Ability Reimagined.
Smoke Testing is all automated, and covers the crucial application flows. These tests could also be considered “End to End”.
 
Words to be more careful with:
End to End testing – This was wrongly used to refer to the Interface testing suite. In practice, many of our regression tests and all of our smoke tests classify as End to End tests.  
Integration testing – This is routinely confused with Interface testing. Many of our Interface Regression tests are also Integration tests, but this is the wrong “catch-all” term. 

