<img align="left" src="https://avatars.githubusercontent.com/u/76134639?s=200&v=4" width="64px">

# My Test Case Manager
A simple flexible XL test case manager for small projects and UAT.  Good for exploratory testing too.
**Version = Excel for Office 365.**

## Table of Contents
 - <a href="#introduction">1. Introduction</a>
 - <a href="#download">2. Download</a>
 - <a href="#gettingStarted">3. Getting Started</a>
 - <a href="#testCases">4. Test Cases</a>


<a id="introduction" class="anchor" href="#introduction" aria-hidden="true"> </a>
### 1. Introduction 
* Do you need to organize and track a small to medium size testing project?
* Do you need to communicate your testing efforts to the project team or a manager?
* Do you need a simple tool to better organize and track your exploratory test results?


If yes to any of the above, then consider using "My Test Case Manager" (MTCM).  MTCM is a lean test tool designed to organize test cases and manage/communicate test results.  MTCM is a simple, minimalist design for software test engineers conducting functional or exploratory testing.  Business analysts can also use MTCM for conducting user acceptance testing (UAT).  You can write the test cases as you execute them, or plan and write them ahead of time.  Run results are tallied and graphed on subsequent worksheets.  You use the report and graphs to communicate status to your project team.  Show them how test cycles work, how test cases are built up over time, how regression testing works with each new build received, how risk is managed from build test to build test, etc.
<br>
<br>

<a id="download" class="anchor" href="#download" aria-hidden="true"> </a>
### 2. Download
To download the "My Test Case Manager" tool (Excel spreadsheet) from this repository's /download folder,
1. [Right-click here with Open in New Tab](https://github.com/DataResearchLabs/my_test_case_manager/blob/main/download/my_test_case_manager.xlsx) 
2. Then click the download button
3. Then click the '...' button at browser Open File popup
4. Then click 'Show in Folder' from popup
5. Then copy-paste "my_test_case_manager.xlsx" file into a directory of your choosing

You should probably save the first copy of "my_test_case_manager.xlsx" as a template that you never alter.  Instead, paste a copy of that file into new project folders and rename the file accordingly (e.g.: "mtcm_project_X.xlsx").

To download examples of the tool in use with sample data from this repository's /samples folder, [click here for samples](https://github.com/DataResearchLabs/my_test_case_manager/tree/main/samples), then click the sample file you want, and finally click the download button.
<br>
<br>

<a id="gettingStarted" class="anchor" href="#gettingStarted" aria-hidden="true"> </a>
### 3. Getting Started
#### General Data Entry Rules
* In general, you only ever edit the pale yellow text boxes<img src="img/img_01_cells_you_can_change.png" width="52">, nowhere else!
* Avoid inserting or cutting rows and cells unless explicitly indicated to do so (i.e.: "Test Run Log" worksheet).
* The dark background cell areas are unused

#### First Open / Security Notice
The first time you open a copy of the .xlsx file in a new folder, Microsoft Office security is going to render the file read-only to protect you.  The screenshot below shows the "Protected View" message (#1).  Go ahead and click the "Enable Editing" button (#2) to open up the file for your use.  Also note that there is *no* VBA code behind this spreadhseet / lightweight "application", so we do not need to worry about enabling macros or code.
<img src="img/img_03_warning_on_first_open.png" width="996">
<br>

#### Setup "Project" Properties
Get started by opening the "my_test_case_manager.xlsm" file, then do the following actions where the numbers in the list below match to the numbered blue dots in the screenshot to the right.<br>
<img align="right" src="img/img_02_enter_project_properties.png" width="524">
1. Click the Properties tab, if not already opened<br>
2. Then, type in your company name, for the report output<br>
3. Then, type in the project or team name<br>
4. Then, type in your name (or multiple analysts if appropriate)<br>
...and now your test project properties are setup.<br>
<br>
<br>


<a id="testCases" class="anchor" href="#testCases" aria-hidden="true"> </a>
### 4. Test Cases
#### Opening "Test Cases" WorkSheet
To open the test case worksheet, click the tab titled "Test Cases".<br>
<img src="img/img_05_click_test_cases_worksheet.png" width="501"><br>
<br>

#### Creating a Section Header
It is a good idea to organize your test cases under sections.  A simple way to make sections is to:<br>
1. Enter "0min" for the "Execution Time" column textbox<br>
2. Enter "i" for Information at the "Status" column dropdown<br>
3. Enter your desired Section Header title at the "Test Steps" column text box.  Also consider making the text bold to standout.<br>
Optionally, set the backcolor of all three cells in the row to your preferred section header color.  In the example screenshot below, light blue was sued for the section header backcolor, but you can choose anything.
<img src="img/img_04_create_section_header.png" width="523"><br>
<br>

#### Writing Your First Test Case
1. First, write in your test steps (callout #1 in screenshot below).  Click the cell, type in your test case details, using Alt+Enter to force new blank lines and make the row taller.  In the screenshot  below, an example multi-line test case is written out (notice the foramtting).<br>
2. Next, callout #2 shows where to set the Status drop down.  Go ahead and set it to "T" for "ToDo" if you are not actually executing the test case right now.  If you are executing the test case as you write it, then pick "P" if it passes, "F" if it Fails, etc.<br>
3. Finally, callout #3 shows where to set the execution time to the number of minutes it took you to write and/or execute this test case depending on what you want to track.  For me, I tend to write and execute the test cases exploratory style for the first test cycle / test run so I combine both times.  Then during regression on subsequent re-runs of the test, I know this Exec Time column value will be substantially less, but at least I accurately captured the  initial write + execute time of test run #1 as well as the execution only tmie of test run #2.  Now that you know how to write one test case, you can write many.<br>
<img src="img/img_06_write_first_test_case.png" width="831"><br>
<br>

#### Excel Formatting
Since the "Test Steps" cell is truly just a single cell (no merging) then the auto-size height works.  Also, the bolding and font color of individual words or lines within the cell as well as all other standard XL formatting will work as expected.  You can even copy-paste a small image or screenshot as expected results into a cell, or paste in several lines of SQL to copy-paste-run as part of your testing.<br>
Note that when using Alt+Enter to increase row height, Excel allows one row to expand up to 29 visible lines of text (I tested); more lines can be present in the row, they just won't be all visible and at some point the cell gets truncated so be reasonable and split test details into multiple rows if needed.<br>
<br>

#### Status Values
There are six possible status values available in the status dropdown show in the image on the left below.  Each status value has conditional formatting applied to set it to an appropriate color.  In the sample screenshot below, each value is displayed with a brief description of how to use each.<br>
<img align="left" src="img/img_08_status_dropdown.png" width="58">
<img src="img/img_07_status_values.png" width="792"><br>
<br>


#### Deleting Test Cases
The simplest way to delete a test case is actually to just highlight the three yellow cells (ExecTm, Stat, and TestSteps columns) for a test case and press the delete key.  In the screenshot below, three test cases are highlighted and will be deleted as soon as either the Delete key or Backspace key is pressed on the keyboard.<br>
Note that it is a bad idea to highlight and delete entire rows, although that should work without impacting automated calculations and graph results; however, it was not tested so steer clear of that.  Ditto for deleting the formula that calculates the Test Case # in column B.


See the advanced section for some easy Search & Replace tips to reset your test case status values for the next Test Run / Test Cycle.
<br>
<img src="img/img_09_highlight_and_delete.png" width="792"><br>


#### Validation Errors
<br>
<br>

#### Current Test Case Metrics
<br>
<br>




<br>
<br>
<br>

### Work these notes into the appropriate sections...
The tool is best used by individual contributors as a local standalone Excel file.  However, I've used it years ago on a test team as a shared file on a network drive or SharePoint...just suggest that you split out each person's work to separate worksheets to minimize collisions.
