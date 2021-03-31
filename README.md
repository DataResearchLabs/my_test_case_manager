<img align="left" src="https://avatars.githubusercontent.com/u/76134639?s=200&v=4" width="64px">

# My Test Case Manager
A simple flexible XL test case manager for small projects and UAT.  Good for exploratory testing too.

## Table of Contents
 - <a href="#introduction">1. Introduction</a>
 - <a href="#download">2. Download</a>
 - <a href="#quickStartGuide">3. Quick Start Guide</a>


<a id="introduction" class="anchor" href="#introduction" aria-hidden="true"> </a>
### 1. Introduction 
* Do you need to organize and track a small to medium size testing project?
* Do you need to communicate your testing efforts to the project team or a manager?
* Do you need a simple tool to better organize and track your exploratory test results?
 
If yes to any of the above, then consider using "My Test Case Manager" (MTCM).  MTCM is a lean test tool designed to organize test cases and manage/communicate test results.  MTCM is a simple, minimalist design for software test engineers conducting functional or exploratory testing.  Business analysts can also use MTCM for conducting user acceptance testing (UAT).  You can write the test cases as you execute them, or plan and write them ahead of time.  Run results are tallied and graphed on subsequent worksheets.  You use the report and graphs to communicate status to your project team.  Show them how test cycles work, how test cases are built up over time, how regression testing works with each new build received, how risk is managed from build test to build test, etc.


<a id="download" class="anchor" href="#download" aria-hidden="true"> </a>
### 2. Download
To download the "My Test Case Manager" tool (Excel spreadsheet) from this repository's /download folder, [click here for download](https://github.com/DataResearchLabs/my_test_case_manager/blob/main/download/my_test_case_manager.xlsx), then click the download button.  Save the downloaded file in a directory of your choosing.  You probably even want to save this first copy ("my_test_case_manager.xlsx") as a template that you never alter, then paste a copy of the file into a new project folder and rename it accordingly (e.g.: "mtcm_project_X.xlsx").

To download examples of the tool in use with sample data from this repository's /samples folder, [click here for samples](https://github.com/DataResearchLabs/my_test_case_manager/tree/main/samples), then click the sample file you want, and finally click the download button.


<a id="quickStartGuide" class="anchor" href="#quickStartGuide" aria-hidden="true"> </a>
### 3. Quick Start Guide
#### General Data Entry Rules
* In general, you only ever enter data into the pale yellow text boxes, nowhere else!  <img src="img/img_01_cells_you_can_change.png" width="52">
* Avoid inserting or cutting rows and cells unless explicitly indicated to do so (i.e.: "Test Run Log" worksheet).
* The dark background cell areas are unused


#### First Open / Security Notice
The first time you open a copy of the .xlsx file in a new folder, Microsoft Office security is going to render the file read-only to protect you.  The screenshot below shows the "Protected View" message (#1).  Go ahead and click the "Enable Editing" button (#2) to open up the file for your use.  Also note that there is *no* VBA code behind this spreadhseet / lightweight "application", so we do not need to worry about enabling macros or code.
<img align="left" src="img/img_03_warning_on_first_open.png"  width="996">


#### Entering Project Properties
Get started by opening the "my_test_case_manager.xlsm"
1. First click the Properties tab, if not already there
2. Type in your company name, for the report output
3. Type in the project or team name
4. Type in your name (or multiple analysts if appropriate)
<img align="right" src="img/img_02_enter_project_properties.png" width="524">





### Work these notes into the appropriate sections...
The tool is best used by individual contributors as a local standalone Excel file.  However, I've used it years ago on a test team as a shared file on a network drive or SharePoint...just suggest that you split out each person's work to separate worksheets to minimize collisions.
