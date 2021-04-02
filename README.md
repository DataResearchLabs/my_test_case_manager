<img align="left" src="https://avatars.githubusercontent.com/u/76134639?s=200&v=4" width="64px">

# My Test Case Manager
A simple flexible XL test case manager for small projects and UAT.  Good for exploratory testing too.<br>
**Version = Excel for Office 365.**

## Table of Contents
 - <a href="#introduction">1. Introduction</a>
 - <a href="#download">2. Download</a>
 - <a href="#gettingStarted">3. Getting Started</a>
 - <a href="#testCases">4. "Test Cases" Worksheet</a>
 - <a href="#testRunLog">5. "Test Run Log" Worksheet</a>
 - <a href="#report">6. "Report" Worksheet</a>
 - <a href="#about">7. "About" Worksheet</a>
 - <a href="#advancedTopics">8. Advanced Topics</a>
 - <a href="#exploratoryTesting">9. Exploratory Testing</a>
 - <a href="#thankYou">10. Thank You</a>


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
#### 3.1 General Data Entry Rules
* In general, you only ever edit the pale yellow text boxes<img src="img/img_01_cells_you_can_change.png" width="52">, nowhere else!
* Avoid inserting or cutting rows and cells unless explicitly indicated to do so (i.e.: "Test Run Log" worksheet).
* The dark background cell areas are unused

#### 3.2 First Open / Security Notice
The first time you open a copy of the .xlsx file in a new folder, Microsoft Office security is going to render the file read-only to protect you.  The screenshot below shows the "Protected View" message (#1).  Go ahead and click the "Enable Editing" button (#2) to open up the file for your use.  Also note that there is *no* VBA code behind this spreadhseet / lightweight "application", so we do not need to worry about enabling macros or code.
<img src="img/img_03_warning_on_first_open.png" width="996">
<br>

#### 3.3 Setup "Project" Properties
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
### 4. "Test Cases" Worksheet
#### 4.1 Opening "Test Cases" WorkSheet
To open the test case worksheet, click the tab titled "Test Cases".<br>
<img src="img/img_05_click_test_cases_worksheet.png" width="501"><br>
<br>

#### 4.2 Creating a Section Header
It is a good idea to organize your test cases under sections.  A simple way to make sections is to:<br>
1. Enter "0min" for the "Execution Time" column textbox<br>
2. Enter "i" for Information at the "Status" column dropdown<br>
3. Enter your desired Section Header title at the "Test Steps" column text box.  Also consider making the text bold to standout.<br>
Optionally, set the backcolor of all three cells in the row to your preferred section header color.  In the example screenshot below, light blue was sued for the section header backcolor, but you can choose anything.
<img src="img/img_04_create_section_header.png" width="523"><br>
<br>

#### 4.3 Writing Your First Test Case
**1. Test Steps:** First, write in your test steps (callout #1 in screenshot below).  Click the cell, type in your test case details, using Alt+Enter to force new blank lines and make the row taller.  In the screenshot  below, an example multi-line test case is written out (notice the foramtting).<br>
**2. Status:** Next, callout #2 shows where to set the Status drop down.  Go ahead and set it to "T" for "ToDo" if you are not actually executing the test case right now.  If you are executing the test case as you write it, then pick "P" if it passes, "F" if it Fails, etc.<br>
**3. Execution Time:** Finally, callout #3 shows where to set the execution time to the number of minutes it took you to write and/or execute this test case depending on what you want to track.  For me, I tend to write and execute the test cases exploratory style for the first test cycle / test run so I combine both times.  Then during regression on subsequent re-runs of the test, I know this Exec Time column value will be substantially less, but at least I accurately captured the  initial write + execute time of test run #1 as well as the execution only tmie of test run #2.  Now that you know how to write one test case, you can write many.<br>
<img src="img/img_06_write_first_test_case.png" width="831"><br>
<br>

#### 4.4 Excel Formatting
Since the "Test Steps" cell is truly just a single cell (no merging) then the auto-size height works.  Also, the bolding and font color of individual words or lines within the cell as well as all other standard XL formatting will work as expected.  You can even copy-paste a small image or screenshot as expected results into a cell, or paste in several lines of SQL to copy-paste-run as part of your testing.<br>
Note that when using Alt+Enter to increase row height, Excel allows one row to expand up to 29 visible lines of text (I tested); more lines can be present in the row, they just won't be all visible and at some point the cell gets truncated so be reasonable and split test details into multiple rows if needed.<br>
Note that any formatting you apply to the Status column will be overriden by the conditional formatting (unless you choose the value "i" which has none).
<br>

#### 4.5 Available Status Values
There are six possible status values available in the status dropdown show in the image on the left below.  Each status value has conditional formatting applied to set it to an appropriate color.  In the sample screenshot below, each value is displayed with a brief description of how to use each.<br>
<img align="left" src="img/img_08_status_dropdown.png" width="58">
<img src="img/img_07_status_values.png" width="792"><br>
<br>


#### 4.6 Deleting Test Cases
The simplest way to delete a test case is actually to just highlight the three yellow cells (ExecTm, Stat, and TestSteps columns) for a test case and press the delete key.  In the screenshot below, three test cases are highlighted and will be deleted as soon as either the Delete key or Backspace key is pressed on the keyboard.<br>
Note that it is a bad idea to highlight and delete entire rows, although that should work without impacting automated calculations and graph results; however, it was not tested so steer clear of that.  Ditto for deleting the formula that calculates the Test Case # in column B.<br>
<img src="img/img_09_highlight_and_delete.png" width="792"><br>


#### 4.7 Validation Errors
In order for all the automated calculations, tables, charts, and reports to properly function, it is important that you fill in all three columns for each test case.  That means every row must have a value for ExecTm, Stat, and TestSteps columns -- no blanks.  If you do leave any columns blank (callout #1 below), the checksum counts will notice the mismatch and trigger  validation errors (callout #2) up at the top of the Test Cases worksheet as shown in the screenshot below.<br>
To correct the validation erros (make them disappear), simply fill in all the blank cells for any partially filled out test case row.<br>
<img src="img/img_10_validation_errors.png" width="1216"><br>


#### 4.8 Current Test Results
The Test Cases worksheet is broken down into two sections:<br>
1. Rows 1-16 are for "Test Results" - a nice summary of counts and test time in a table with a graph.<br>
2. Rows 17-319 are for "Test Cases" - where all the details go.

These metrics automatically update as you write and execute test cases below.  They summarize all the results on this worksheet.  If you copy-paste the worksheet to make a second or third instance, then each will have their own self-contained Test Results section.<br>
I like to screenshot this section for status emails sometimes, to give a pretty summary of where the current Test Run / Test Cycle is at.  This is especially nice for when you are partially thru a test run and can show not only the actual time completed ("B"locked + "F"ailed + "Q"pass + "P"ass), but also the expected remaining time ("T"odo) because in theory you have the prior execution times still in place from your last run...or you've entered the expected time to execute in.<br>
<img src="img/img_11_test_case_results.png" width="383"><br>
<br>
<br>


<a id="testRunLog" class="anchor" href="#testRunLog" aria-hidden="true"> </a>
### 5. "Test Run Log" Worksheet
#### 5.1 "Test Run Log" Levelset
To open the test run log worksheet, click the tab titled "Test Run Log" (callout #1 below).<br>
This form is used at the end of every Test Run (Test Cycle) after you're done executing all the test cases from the prior worksheet.  You simply transcribe the automatically calculated totals from the Test Results table (in cells J5 thru J9 from the upper right section of the Test Cases worksheet) into the appropriate cells on this worksheet.  Likewise, you transcribe the defect counts from your defect system (typically a website like Jiri or any other bug tracking tool).<br>

There are a few key points here that need to be emphasized:

1. You are manually entering these values when a test run / test cycle is completed.<br>
2. These values drive the Report worksheet to the right.<br>
3. You enter test case status counts taken from the "Test Cases" worksheet
4. You enter defect counts taken from your Defect system (some other web application most likely)<br>
   However, you could track failed test cases as defects manually in the sections below if necessary.<br>


#### 5.2 Inserting Test Run Rows
The general process for entering Test Run (test cycle) row data is as follows:<br>
1. First, enter **Test Run #1** results in row R1 that comes default (callout #2).  At this point, the report will **not** have a trend.<br>
2. Next, enter **Test Run #2** results in row R2 that comes default (callout #2).  At this point, the report **will** have a trend.<br>
3. For **Test Run #3** and beyond (regression), follow the instructions in blue text (callout #3) to insert a new test run.  It is important to copy and then insert paste the last line on top of itself, pushing itself down a row.  This maintains all the automated reports and charts, so the series automatically resize and you only have to change the values in the lowest row that was pushed down.  I will demo this in the YouTube training videos (showing is easier than describing).
<img src="img/img_12_test_run_log_levelset.png" width="956"><br>


#### 5.3 Entering Test Run Values
It is important that you properly fill out all of the columns for each Test Run / Test Cycle row.  Only enter values into the pale yellow cells (leave the calculated silver cells alone).<br>
Here are the column definitions and suggestions about how you should use them:<br>
1. **Run #:** This is the Test Run or Test Cycle Number.  Use "R1", "R2" style formatting.  A Test Run or Test Cycle is as complete a pass thru executing the test cases as you can possibly do for a given build or release or at a given point in time.  Use sound judgment in determining when to start and stop a Test Run or Test Cycle.<br>
2. **Test Run Description:** The name you give a Test Run (or Test Cycle) is important.  It helps tell the story of how and what you tested and what issues you ran into.<br>  Management and others on the development team often believe testing is simple and linear. *"There's 60 test cases, they _should_ take 1 minute a piece, so why aren't you done in 60 minutes?"* <br>
By properly naming and organizing your test cycles, you can help educate your team on how there are multiple test runs, the scope grows as does your understanding and available tests to run.  Example names might be "Sprint 05", or "Release 2.3", or "Week 14", or "UAT for Project X", etc.<br>
3. **Date:** Use the date the test run was completed.<br>
4. **Execution Time (hr):** Enter the total execution time as automatically tallied back in the Test Cases worksheet.  If you copy-pasted multiple Test Case worksheets, then use a formula here to sum those values together.<br>
5. **Test Cases:** Enter the ToDo, Block, Fail, Qpass, and Pass counts as automatically tallied back in the Test Cases worksheet.  If you copy-pasted multiple Test Case worksheets, then use a formulate here to sum those values together.<br>
6. **Defects:** It is up to you to either track here or fetch from your defect system the following counts:
   * **Open, ShowStoppers:**  This is the count of high priority/severity issues that will block release
   * **Open, Allow:** This is the count of low-medium priority/severity issues that can ship/deploy
   * **Defer:** This is the count of deferred defects where a decision was made to ignore for now
   * **Closed:** This is the count of fixed/retested/closed defects
<br>


<a id="report" class="anchor" href="#report" aria-hidden="true"> </a>
### 6. "Report" Worksheet
#### 6.1 Introduction
The "Report" tab is very important.  You should use screenshots of these graphs to communicate yuor testing status, or story, to the project team and to management.<br>
* It is nice to be able to depict that testing is not a single pass, single dimensional event; but that there are multiple releases that need to be tested.<br>
* It is nice to depict the impact to schedule that blocked test cases have had when they are finally tested and yield high defect rates.<br>
* It is nice to show the risk that qualified passes on regression tests to meet a deadline have to the final release.<br>
* It is nice to show the actual execution time in hours it takes to test each test cycle (release, sprint, group of builds, etc.).<br>
* It is nice to show how the actual execution time tapers off once test creation is done and you are simply regression testing (execution) only.<br>
* It is nice to plan the final release around stability, where there have been NO show stopper defects in the last two releases, and mininmal (or no) "allowed" (low priorit) defects.<br>
* It is nice to to keep a list of defects organized in three buckets (Currently Open, Closed-Since Last Report, Closed-Older) so that you can copy-paste them into a weekly status report email.<br>


#### 6.2 Report Header
The report header shows the company  and project names at the upper left section of the report.  These are the same values entered in the Properties tab.  The right section of the report headers indicates which Test Run / Test Cycle (e.g.: "R6") that is currently being displayed.  The tester's name (also from the Properties tab) is also displayed in this section.  The total test case count and total defect count is also tallied and displayed in the right side of the report header.
<img src="img/img_13_report_header.png" width="847"><br>


#### 6.3 Test Case Count Graphs
<img align="right" src="img/img_14_report_test_case_counts.png" width="446"><br>
The test case count graphs are located on the left half of the page, directly below the report header.<br>
* There is a **snapshot graph** on top depicting the counts for the latest release (R6 in our example below).  
* Below that is a **trend graph** showing test case results over time.
  
In the snapshot graph below, The dark green tells me that 26 test cases were executed and passed on this final R6 Test Cycle.  It also tells me that 104 test cases were Qualified Passes, which typically means they passed on a prior Test Cycle, but due to time constraints we did not regression test them again on the latest test cycle.  At a glance, I can see our risk exposure that for every one test case we executed and passed in R6, there were 4 that we skipped based on a prior test cycle pass.  If the project team and management believe quality is important, then we can ask to do a full regression test by executing the 104 QPasses.  Furthermore, we can tell them exactly how long it will take by pulling the ExecTm value off of the most recent "Test Results" graph back on the "Test Cases" worksheet.  Makes for better decision making all around.<br>
I can also see in the trend graph that the number of blocked and failed test cases started off high, then tapered off as the project stabilized.  I can also see that from R4 thru R6, we increasingly relied upon qualified passes to meet deadlines (rather than executing full regression coverage).


#### 6.4 Defect Count Graphs



#### 6.5 Test Case Execution Time Graph




#### 6.6 Releasability Graph



#### 6.7 Defect Details - For Status Reports



<br>
<br>


<a id="about" class="anchor" href="#about" aria-hidden="true"> </a>
### 7. "About" Worksheet
<br>
<br>


<a id="advancedTopics" class="anchor" href="#advancedTopics" aria-hidden="true"> </a>
### 8. Advanced Tips & Tricks
<br>
<br>
Advanced (Don't forget to write these up):<br> 
* "Jump Stops" using ctrl + arrow keys in columns A or F.<br>
* Sample SQL embeddd in a test case<br>
* Sample Screenshot expected results<br>
* Sample with multiple Test Case worksheet tabs (300, 600, 900 test cases)<br>
* Sample Multi-User Shared Workbook<br>
* Conditional Formatting Mess if you Copy-Paste + How to Fix<br>
* Other...<br>
<br>
The tool is best used by individual contributors as a local standalone Excel file.  However, I've used it years ago on a test team as a shared file on a network drive or SharePoint...just suggest that you split out each person's work to separate worksheets to minimize collisions.<br>


<a id="exploratoryTesting" class="anchor" href="#exploratoryTesting" aria-hidden="true"> </a>
### 9. Exploratory Testing
<br>
<br>


<a id="thankYou" class="anchor" href="#thankYou" aria-hidden="true"> </a>
### 10. Thank You
<br>
<br>
* History from V1 thru V5 spanning multiple prior hobby sites (PBSys, WinTestGear, etc.)







