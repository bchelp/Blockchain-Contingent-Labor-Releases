# Blockchain-Contingent-Labor-Releases
<h3>02/03/22 Release</h3>
</p>
Contractors – Timesheet PO select – Contractors who have more than one PO have the option to select which PO they need to claim against.  We changed 2 step PO selection process (select PO and press go) to be a single step (select PO) when choosing which PO to claim time against on the Timesheet page.  
</p>
Preparation for UK expansion – Contingent Labor on IBM Blockchain has been a US based application since 2018, but we will be expanding to the UK in February 2022.  There has been a lot of work in the background to prepare for this expansion.  This release completes the bulk of the code changes required to onboard UK Purchase Orders into the system. 
</p>
There may be some differences in the data layout on the pages to accommodate for the expansion.  
</p>
Timesheet table – There are 2 new columns in the timesheet table, SD (stand by) and CO (call out).  Both relate to the hour types available on UK timesheets.  These columns will be blank for all US timesheets.
</p>
Invoice Reconciliation page – We reorganized the data on the Invoice Reconciliation detail page to group the data into a table format to standardize the look and feel on that page.
</p>
<h3>01/05/22 Release</h3>
</p>
Timesheet Copy Claim Codes – A new function was added to allow contractors (and suppliers) to COPY claim codes from a previous timesheet to the current timesheet. This enhancement will help contractors who are switching POs and don't have an automatic default of their previous ILC claim codes to their current timesheet when their new PO starts. Only ACTIVE claim codes will copy into the new timesheet, a warning message will inform contractors of claim codes that could not be copied into the new timesheet based on claim code validity.  Hours will not be copied, only claim codes.
</p>
Timesheet status – The status of the timesheet is now listed at the bottom of the timesheet detail page. We have replaced the text of who has already verified to match the timesheet status in the table view thereby being clearer about who is left to act on verifying each timesheet.
</p>
Non-Billable totals – To more readily see the total hours claimed by ILC users to NON-BILLABLE accounts (either non billable ILC accounts like ATCONOFF, or to custom line items provided by the supplier which are non-billable to IBM), there is now a timesheet total row for Non-Billable accounts. If a Non-Billable ILC account was claimed as ST, those hours will show in both the ST total rows and the Non billable totals row but will not impact the total billable hours being claimed.
</p>
CARBON forms for Contractor Record- Managers, CCAs and SAMs will notice a new look and feel to the data they are entering into the Contractor records. We are continuing updating our application to be using CARBON, so the layout of the contractor record “My Edits” tab will have the new look and feel, but all the same fields and functions.
</p>
Table Spacing - UI enhancement – The column spacing on ALL tables were adjusted to better optimize the column widths to see more information on a standard screen.
</p>
Correction timesheet – There is a NEW column in the timesheet table that shows if the timesheet has a submitted correction in the Post Processing timesheet section of the timesheet. This true/false indicator will inform users if the original timesheet was submitted, fully verified, invoiced and is now being re-submitted with corrections.
</p>
Tour Guide – New Contractors will be presented with a tour of their timesheet upon initial log in when they press Claim Time. This is to highlight the different areas of the timesheet and a quick overview of what to expect when claiming time in our application.
</p>
</p>
<h3>**2021 Highlights**</h3>
<h3>11/09 Release</h3>
Timesheet details – UI enhancement – Timesheets have been modified to maximize the timesheet information shown on a single screen to minimize scrolling.  This modification collapsed some of the Contractor details and changed the calendar picker format.  Please see updated training documentation for more details.
</p>
Duplicate timesheets – Contractors with more than one active PO may try to submit a timesheet for the same week under both POs.  To prevent accidental duplication of timesheets, there is now a WARNING pop up message that asks the contractor to confirm that they intend on submitting a second timesheet for the same week noting that a timesheet was already submitted and providing the PO number for the timesheet already submitted.
</p>
Editing timesheets – Contractors needing to edit their previously submitted timesheet will now see a pop-up warning message asking them to confirm. Pressing “Make Edits” or “Make Corrections” puts the timesheet back into a SAVED status.  To prevent this from happening unintendedly, the pop-up warning is now in place instructing the user that the timesheet will be in a saved status until resubmitted. 
</p>
Timesheet Page – UI enhancement – The column spacing on the timesheet table was too wide and didn’t easily allow users to see their full details without scrolling left and right.  The timesheets table was updated to better optimize the column widths to see more information on a standard screen.
</p>
Timesheet Page Pending tab - Managers and DTVs will now be defaulted to their PENDING tab on the timesheet table page instead of their escalated tab.  While both tabs will remain, we received feedback that the preference will be to be defaulted to the PENDING tab upon navigation to the Timesheet page. 
</p>
Manager/DTV dual role – With this release, managers that have a DUAL role of manager and DTV will now be able to change their role without logging out.  The ability to toggle between roles is available by clicking on the username/role listing at the top right corner of the app.  See updated training documentation for more details. 
</p>
User Help – Ever needed the link for our training slides?  We have now updated our USER HELP page to include the links to all our training guides as well as links to our SLACK channels for questions that cannot be answered from the guides.
</p>
</p>
<h3>10/07 Release</h3>
Timesheet FONT – Based on feedback from users, we have changed the font on the timesheet page to be darker and a bit larger and more consistent in sizing. 
</p>
Low Funds Dashboard – Manager and Supplier dashboards now have a Low Funds tile.  Low funds is defined as less than 20% of funds remaining on ANY of its line items (Standard Time, Over Time, Double Time or Expense).  Clicking on this tile will bring you to the Remaining Funds report which will give you details on which PO and which fund category is low. 
</p>
Automated Contractor revoke – Managers and SAMs will now receive weekly notification emails of contractors whose Serial number is no longer valid in IBM’s Bluepages.  If the contractor is still performing work for IBM, their DRMS record will need to be corrected so there is a valid entry in Bluepages.  If by the following week they still do not have a valid blue page entry the contractor will be revoked from the Contingent Labor on IBM Blockchain application.
</p>
Automated Manager/DTV revoke – Manager and DTV will automatically be revoked from the Contingent Labor on IBM Blockchain application if their Bluepages record is not valid using their ibm.com id.  
</p>
Reports – As we continue to update our User Interface to utilize Carbon, we have updated the look and feel of the reports available from the “Reports” page.  Same functional to the reports, just a new user interface. 
</p>
Invoice Report – In addition to the carbon change, we have added the Invoice Reconciliation status to the INVOICE report output.  
</p>
Contractor Search – We have enhanced the search function on the Contractor Records page to allow searches by Contractor Status.
</p>
Edge browser- Our application was previously not supported by older versions of Edge.  Now that Edge’s has released Edge Chromium, we have removed the warning message the Edge is not a supported browser.  
</p>
</p>
<h3>08/25 Release</h3>
Logon page – With the transition to Kyndryl, some of our users will be using their Kyndryl emails to log on.  The “Sign in with IBMid” button was removed.  Enter in your email address into the user name, if it is part of the IBM domain you will be routed to IBM’s SSO when pressing NEXT.  If the username is part of the Kyndryl domain, you will be routed to Kyndryl’s SSO when pressing NEXT. 
</p>
Timesheet table - Timesheets displayed on the timesheet tab will now be sorted by Timesheet Weekending date with the most recent timesheets at the top of the table.  You still can change the sort order to a different column if needed.
</p>
Timesheet table – We have added the ability to select the number of records you would like to display on the timesheet table.  This will allow you to select more timesheets at one time for CSV download or bulk verification. 
</p>
Timesheet detail, SAM email – Contractors are not able to adjust their timesheet hours once their timesheet is fully verified.  Only the supplier can do this on the contractor’s behalf.  To help the contractors know who to reach out to if hours updates are required, we have added the Supplier (SAM) email hotlink to the timesheet status message above the Make Edits button. 
</p>
Contractor Country Code – As we continue to expand our application, we need to support cross boarder contractors where the contractor’s bluepages country information may not match the PO’s country code.  To allow for the necessary bluepage validation to work correctly, we have implemented a NEW field in the Contractor Record called Enterprise Directory Country Code.  This is the 3 digit country code suffix of the CNUM in blue pages.  This will default to the country code of the PO, for the US this is 897.  This country code CAN be updated if the contractor is working on a PO for a country that does not match their Bluepages record.   (Cross boarder -Example US based PO but employing a contractor from Canada)
</p>
ILC failures – Enhanced Timmybot failure messaging.   – ILC enabled contractors and their managers receive automated emails from timmybot stating if ILC accepted or rejected the submitted timesheet.  For failures, we have updated the failure messaging to include likely corrective action steps.  The bchelp team will NO LONGER send individual emails about each ILC failure.  The corrective action should be available to you in the failure notice from timmybot.  Please read the actions and resubmit once updated so your time can be added to ILC successfully. 
</p>
Invoice Recon Manual Reprocess function - Financial Analysts can now manually reprocess an Invoice Reconciliation record. This function will allow the invoice reconciliation record to pick up any later verified timesheet or timesheet corrections and reflect the correct hours verified in blockchain. </p>
</p>

<h3>07/24 Release</h3>
User Experience - Contractors logging in on Friday nights are now directed to current week’s timesheet based on their browser timezone. Previously contractors logging in later in the day on Friday may have experienced being presented the “next week’s” timesheet because system time had already rolled to Saturday. This enhancement will keep the user being defaulted to the current week until MIDNIGHT on Friday night according to their browser timezone.
</p>
User Experience – We have fixed the sorting function on the Contractor Record table where you can now sort by the USER NAME correctly.
</p>
New Notification – There is a new weekly email that will be sent to Managers, Contractors and Supplier Account Managers to inform them of timesheets that have NOT been submitted. The report covers the timesheets that are “missing” within the last 6 weeks for any contractor whose contractor record was All Approved during that 6 week time period and did NOT submit their time. (Saved timesheets are considered not submitted).
</p>
Error prevention – Purchase Orders are 1 contractor per 1 PO, as such we have removed the ability to add 2 contractor records to a single PO and have added error handling to prevent accidental creation of a duplicate record due to timing or sync issues.
</p>
Invoice – We have added the Buyer Contractors ID to the Invoice data for easier cross reference. This can be seen in the Invoice Reconciliation, Supplier Invoice and Blockchain invoice pages.
</p>
Invoice - We added the hours type breakdown to the download of the Invoice tables as well, so you can see the hours types that were used more readily.
</p>
European Expansion - In preparation of our expansion beyond US based POs, we are making some updates to our application. You will now see the Unit of measure show on PO details by line item. This is to account for other countries use of Professional Working days so their rates are not all hourly.
</p>
European Expansion -Supplier Admins will also see that there is a new column in the invoice calendars to denote if the calendar is monthly or not. The ability to select monthly is available for UK, therefore all invoice calendars created for the US will say Monthly = FALSE
</p>

<h3>06/19 Release</h3>
Kyndryl  - We have taken steps to prepare our application for the spin off of the GTS-IS business from IBM to Kyndryl, scheduled for **September 1, 2021**.  Kyndryl employees and contractors shifting to Kyndryl will still be using the Contingent Labor on IBM Blockchain application for time entry and verification.  This release we prepared to handle the user creation and set up of NEW contractor records against the Replacement POs which will be issued for Kyndryl.  This automation will help with the transition process and reduce the manual effort for both managers/CCAs as well as Suppliers (SAMs).
</p>
Kyndryl timesheets – On the go live date for Kyndryl, we have taken steps to prevent contractors from claiming time against their IBM PO after the 9/1 date and only allowing them to claim time against their Kyndryl PO to avoid timesheet and invoicing errors to the wrong company.  Details can be found in the contractor, manager and SAM training documentation. 
</p>
Log on error message – As new contractors or managers try to log into the application, if their user ID is not yet set up they are presented with an error message.  We have added to this error message useful information on why they may not yet have access and how to resolve if possible. 
</p>
European expansion – As our application is preparing to expand to countries outside of the US, the use of country code will become more important.  This release we have added the country into the Invoice Calendar definitions.  SA (Supplier Admins) setting up new invoice calendars or modifying existing invoice calendars will now see the country has been added.  For now it is all still US based but these are steps we are taking to prepare for expansion. 

<h3>05/25 Release</h3>
SEARCH - As we continue to roll out Carbon components, this release sees a new enhancement to the SEARCH function. Searching tables with the spyglass icon you can use the PLUS symbol to add a new search filter.  The Carbon filtering is more crisp, easier to navigate and provides Boolean selection for our true/false fields to reduce typos. 
</p>
FILTER ICON - You will now see an indicator on the tab for which you have filtered data indicating some data may not be displayed. Filter icon will clear once the filters are removed.  As you switch tabs, the filtered icon will only show on the active tab, but if you return to a tab where the filters are still applied the filter icon will show up again.  
</p>
TIMESHEET TABLE – The timesheet tables will now display the breakout of billable hours between hours categories (ST = Standard or Straight Time, OT = Overtime, DT = Doubletime).  This information is available in the table downloads as well as showing on the User Interface. 
</p>
INVOICE FAILURE REASON CODE – For our Financial Analyst teams, a new feature has been added to allow failed invoices to be categorized with a failure reason code to aid in analysis.
</p>
PREPARATION for Kyndryl - As the spin date approaches where GTS will separate to become Kyndryl, we are making changes to our application to allow for both IBM and Kyndryl data to exist in the same blockchain application. This release contained work to prevent Kyndryl contractors from claiming time against their POs prior to the **September** 1 Day0 date.  Most of these enhancements will not be visible to IBM, but we are working hard to prepare the Contingent Labor on IBM Blockchain application to support both IBM and Kyndryl. 
</p>
</p>
<h3>05/05 Release</h3>
Password Change - To comply with ITSS standards for passwords, passwords will need to be updated every 90 days. This applies for all users not using w3ids where password reset is controlled by IBM's SSO. Users will be warned 7 days prior to password expiration and prompted for password update.  Once expired, users will be forced to change their password prior to logging on and will be taken to the password reset page upon an attempt to log on.
</p>
Planned Maintenance Notification - With this release we will now have the ability to notify users of upcoming releases or maintenance windows prior to taking system down and putting up maintenance page. Informational messages will be viewable upon logging into the url and will appear for every log on until the maintenance window begins.  
</p>
Contractor Dashboard - Contractors have a new landing page in our application. The Contractor dashboard gives greater visibility to contractors if they have SAVED or Rejected timesheets that require their action, and visibility into timesheets still pending verification.  
</p>
Archive Timesheets - Contractors and SAM (Supplier Account Manager) can now archive SAVED timesheets. This will allow contractors to clean up their saved timesheet view if a timesheet was created and is now no longer needed.  Archiving a timesheet removes it from the timesheets tables for all persona (Contractor, Manager, SAM, DTV, FA).  These archived timesheets are not eligible for payment to the contractor or invoicing to IBM.  There is a way to restore an archived timesheet if the timesheet was archived in error and now needs to be submitted.
</p>
Searching ST Hours - Managers, CCAs, FAs and SAMs will see a new search function to allow you to search Purchase orders by Remaining ST hours with less than or equal to the hours searched
</p>
Reports - For the SAM (Supplier Account Managers) who will be able to see purchase orders for both IBM and Kyndryl, we have added to SAM report functions the ability to filter by the company name (either IBM or Kyndryl).  Report results include the company name in the report results. 
</p>

<h3>04/20 Release</h3>
Email upgrades - This release you will see a new look and feel to the emails that are sent out by the Contingent Labor Blockchain application directly.  Emails like timesheet verification, PO delegation, etc will all have a new standardized format and will look a lot more official.  
</p>
User Interface Changes - We are working on changing our UI to be based on CARBON.  This release you will see a change in the banner messages presented to users when performing actions within the application.  These banner messages more closely aligned to the standard with other IBM applications.  You will see that success messages automatically close after 7 seconds, while informational, warning or error messages require your acknowledgment of the message.  Messages will also stack on the right-hand side of the application so you can see more than one message at a time.
</p>
ILC Non Billable accounts - For those contractors who are ILC enabled and are using a select set of Non Billable account codes to claim "Time Away" on their timesheets, these claim codes are now considered NON BILLABLE and therefore will not be included in the Total Billable Hours.  The hours will still be transmitted to ILC but will not be included in the total billable hours listed on the timesheet, nor will they be included in invoicing from the suppliers.  (examples of such work items are: ATCONOFF, ATQNOBIL, NONBILLCT, UNBILLCT, ATUNBIL2 and ATQNOBI1). This does NOT change the behavior of the vacation code used by many contractors with Account = SK00, Work item = FPSUBZER where zero hours are claimed.  
</p>
Preparation for Kyndryl - IBM announced that our new spin off company name is Kyndryl.  For those people transitioning over to Kyndryl, we will continue to support both IBM and Kyndryl within our same Contingent Labor on IBM Blockchain application.  As both IBM and Kyndryl will exist within the same application, our Suppliers (SAM) will need the ability to distinguish between both companies.  We have added "Company Name" indicators to the SAM view for all tables and detail records (PO, Contractor records, timesheets and Invoices)
</p>

<h3>3/16 Release</h3>
Performance - This release was focused around increased performance in bulk tables, both being to load and extract tables across the application. Users should see tables loading more rapidly and being able to view the whole table without an error being presented.  With the aggregation that was originally in the application, users were finding the tables were either not loading or were taking a long time to load.  Our Dev team made updates and you should see a performance increase in all bulk tables. 
</p>
User Interface Changes - Corrected UI SORT issue, when on a table and using the sort function while not on page 1, this correction will now bring you back to page 1 to see all the data sorted.  Additionally, the title header now will stick with the main header so while you are scrolling vertically, you don't lose what page you are on (Contractor/Timesheet/Purchase Order)
</p>
Emails - Every week we send an email to the managers to notify them of POs that are expiring.  This notification had incorrectly notified managers of Expired POs that were already in the status of CANCELLED POs, we have removed the CANCELLED POs from these emails to remove confusion. 
</p>
Consistency - To continue with our remaining of the IBM Serial number and IBM Contractor ID to be Buyer Contractor ID, we have updated the output of all reports to list the output as Buyer Contractor ID. Same reports all still have the same function, just updated the labels to be consistent.  This is still referring to the 6-digit serial number listed in blue pages.
</p>
Documentation - We updated all our PDF documentation to have screenshots matching the new UI Carbon headers, and all changes up till this release.  Links to the training documentation are available on the Release Notes on the application UI. 
</p>

<h3>3/04 Release</h3>
User Interface Changes - We are working on changing our UI to be based on CARBON, this release you will see a change in the headers and menu selection.  These are a sleek black header which is more standard with other IBM applications.  We removed the action tray icons as they were no longer necessary after implementing the manager and SAM dashboard and providing tabs for pending actions.  The timesheet verification queue icon will appear in the header only when there are timesheets processing in the queue.
</p>

Contractor serial number - We have standardized references to the contractor's blue pages serial number across the application.  It had been listed as both IBM Serial Number and IBM Contractor ID.  We have changed the name to be reflective of the supplier/buyer relationship in our application, so it is now referred to across the application as "Buyer Contractor ID".  This doesn't change its functionality, it still refers to the 6-digit Blue Pages serial number, just with a consistent name. 
</p>
Calendar - The Date Picker calendar icon now only displays available dates up to the date of the PO expiration.  This was the final piece to the removal of the Grace Period.  Now the calendar on the timesheet page clearly indicates the ending period of the PO.  While the contractor can still claim time for the whole week even if the PO expires in the middle of the week, the calendar will clearly show the PO end date.
</p>
Expiring POs - We updated the access on the Expiring POs tab for both Managers and SAM (Supplier Account Managers) to allow them to move a PO from their Expiring Tab to their Inactive tab without having to navigate back to the Primary tab to do so.  You can now move directly to the INACTIVE tab from the Expiring tab.
</p>

<h3>2/23 Release</h3>
User Interface Changes - We are working on changing our UI to be based on CARBON, in preparation for that we have standardized the fonts and colors of the User Interface.  Users will notice a darker font, the IBM Plex font and more standardized color scheme.  In addition to the font changes, the "FEEDBACK" button was nudged away from the vertical scroll bar to not block its usage.  This was based on customer feedback. 

SSO log on - For our users that log in with their IBM ids, we have upgraded our SSO log on to the NEW w3id SSO on IBM Security Verify (ISV).  

We have extended the information that our DTVs (Delegated Time Verifiers) can view.  They are now able to view the contractor record table and details.  This will allow them to have a better visibility to the POs under which contractors are claiming as well as the PO end dates.  There was added training documentation for the DTVs.

Contractor record updates - We have added the Manager, DTV and Supplier (SAM = Supplier Account manager) emails in the contractor full record details.  This will better allow you to reach out the approving parties and have visibility to whom contractors are assigned. 

Timesheet updates - We have added the "latest submission" date to the timesheet detail.  We have had multiple requests to have this information available to the verifiers.  You can see what date the timesheet was last submitted for verification on each timesheet now. 
Additionally, we have tried to add more clear pop up reminders in the Corrections/Post Processing timesheet to remind people that this is a CHANGE from the original, not a replacement for the originally submitted timesheet. 

Warranty Enhancement - In our previous releases we had implemented a feature for certain suppliers to be able to warranty a contractor.  The enhancement this release is to allow timesheets that may have had a supplier invoice to be warrantied IF an invoice reversal was submitted netting the supplier invoice to zero dollars on all lines.  

Supplier Invoice and Invoice reconciliation - Updated the supplier invoice SEARCH capabilities.  The Date search was fixed, and additional search capabilities were added to allow for narrowing down the invoice data for analysis.  


<h3>2/11 Release</h3>
RELEASE NOTES
In addition to the Grace period removal, we are implementing a feature to display the "Release Notes" on the UI, so you will be informed of the updates to the application when logging in for the first time after the release, or on demand by navigating to the "Release Notes" drop down.  

</p>
GRACE PERIOD REMOVAL
Per the direction of our product owner and procurement business we are now REMOVING the grace period that had been established within our application to allow contractors to claim time for 28 days past their PO end date, or to submit timesheets against a PO for up to 4 weeks beyond the date that the PO was exhausted of Standard Time funding (managers could not verify these timesheets but contractors were allowed to submit).  This was originally implemented to allow time for the managers and Support Squads to initiate the PO renewal process so contractors could keep working.  It was not meant to be a permanent solution and it is now time to remove this Grace Period from our application and return to enforcement of procurement rules where contractors should only be claiming time to POs that have funds and are within their validity period. 
</p>
INVOICE UPDATE - REJECTION INVOICES
Invoice Update for Financial Analysts to pull in the billing period for rejection invoices which will allow for supplier submitted rejection invoiced to be automatically reconciled with the Contingent Labor Blockchain application.
</p>
<h3>1/20 Release</h3>
We added the ability to download a PDF of time sheets. This is especially helpful when there are many accounts and a screenshot will not capture the whole screen.

Warranty Contractor process established for select supplier (CTG) - this enhancement allows Managers to initiate a warranty process for contractors who left during their warranty period. Their time sheets will be flagged so IBM knows they are non-billable, and the contractor won't be able to submit more time sheets.

Supplier invoices will now include the Payment Due Date, Paid Date, and Payment Document Number 

<h3>2020 Highlights</h3>

We added a timesheets page allowing contractors to see a table of ALL of their timesheets, including saved (not submitted) timesheets and timesheets on multiple POs

In response to manager feedback, we created a new landing page which clearly presents all of the items awaiting action.

We introduced a variety of reports that allow Managers, Delegated Time Verifiers, Financial Analysts, IBM Contractor Administrators, and Suppliers to keep track of and have better insight into their contractor and Purchase Orders.

Weekly emails to remind Managers and DTVs about time sheets that need to be verified

Made it so that if there is a renewal PO that flows to the app and is linked in CSA to a PO already in the Blockchain Application with an "All Approved" contractor record, the contractor record on the new PO will automatically be created.

New tab added to Purchase Orders page: "Pending Contractor Assignment"- this tab will show the new and renewal POs loaded to the application that do not yet have a contractor associated to them.

Made it so that when a new timesheet is loaded, we will only copy over the valid timesheet rows from the previous week's timesheet.

Upgraded to IBM Blockchain Platform (IBP) v2

<h3>12/3 Release</h3>

Invoice reconciliation will now be based on hours rather than value. Previously the blockchain invoice value in terms of currency (dollars for the US) was compared with the actual invoice the supplier generated. Now, it is the hours that are being compared which allows reconciliation to pass even when certain edge cases like additional taxes would have caused reconciliation to fail in the past

We updated the Missing Timesheets Report to take all the contractors previous POs, active or inactive, into account when displaying the list of time sheets that are missing for a given week

<h3>11/9 Release</h3>

New report to identify contractors who are missing timesheets in a specified time period

Added visibility of Saved (Unsubmitted) timesheets under the "All" Timesheet tab

<h3>10/27 Release</h3>

**Now using fields from upstream systems to automatically delegate POs to the correct Manager and Delegated Time Verifier- will reduce onboarding time** | 
Manager email and Delegated Time Verifier (if applicable) are now required fields in the upstream systems we pull our PO data from, so we are utilizing this to automatically delegate POs to the correct managers and assign the  

**Now keeping track of "real-time" funds on the PO to govern time sheet verification** | 
Once a Purchase Order is pulled into our app from BDW (our SOR), we will take a snapshot of the number of hours and expenses available on the Purchase order, creating an "internal value" for our application. From that point forward, when a time sheet is fully verified, the hours will be subtracted from this value, and likewise for expenses. Rejected time sheets will not affect this internal value. A time sheet cannot be verified by the manager or supplier if it will cause the internal value to become negative. 

**Time Sheets that were locked due to having been invoiced can now send to ILC correctly** | 
Once a time sheet is marked as having been invoiced, that time sheet is locked in the Blockchain application. Changes to the time sheet must be made as "Post-Processing Edits" where the changes are made as positive or negative "delta" values. Because of the complexity of working with these delta values, changes to the ILC codes made after invoicing would have to be submitted in ILC directly, but now, we will tabulate the new totals and send the updated overall values to ILC. 

**Accessibility enhancements** | 
We are trying to make sure our app stays compliant with accessibility standards so that everyone can use our application regardless of any impairments they may have 

**Defect with not being able to clear Notifications resolved** | 
There was a defect where the notifications under the bell icon could not be cleared. We have resolved this and you should be able to clear individual notifications or clear all notifications that are visible on the page

<h3>9/1 Release</h3>

When switching tabs, instead of reloading the full page and presenting a loading symbol in the middle of the page, we'll present the loading symbol in just the tab that is being loaded.

We received feedback that on certain monitors, the font on the time sheet page was difficult to see and lacked contrast. In response to this feedback, we've increased the boldness of the font so it is easier to read.

In response to manager feedback, we created a new landing page which clearly presents all of the items awaiting action. There are four main components:

The time sheets which are pending your verification
The contractor records which are pending some action on your side to be fully set up
New POs that have come in but do not have a contractor record set up against them
POs which are expiring within the next 8 weeks and thus could necessitate a renewal PO if the contractor is to continue working.
Once any of these four is zero (meaning you have no pending action), the text will turn from red to green for that component.

We added a new Expiring tab on the Purchase order page which shows all POs where the PO will end within 8 weeks of the current date. This is a heads up to you about the POs for which you need to work on a renewal due to the upcoming end date.

The Inactive PO and Contractors tabs will now be tied. When you move a PO to inactive, any contractor records associated with the PO will also move to the inactive tab, and visa versa

Contractor start and end date now shows up in the csv export of the PO table

**Reports!**

We introduced a variety of reports that allow Managers, Delegated Time Verifiers, Financial Analysts, IBM Contractor Administrators, and Suppliers to keep track of and have better insight into their contractor and Purchase Orders. The Reports can be accessed through the menu in the top right corner of your screen.

**Contractors Not Claiming**: This report shows all contractors that
- Are within the start and end dates on their PO
- Are in "All Approved" status
- Have not been moved to your inactive tab
- Have not yet submitted a timesheet in the blockchain app

**Remaining Funds**: This report shows a list of all POs that have 20% or less of funds remaining on any of the line items, for POs that are not on your inactive or cancelled tabs.

**Expiring Contractors**: This report shows a list of contractors that are 8-weeks or less in advance of the contractor end date, that are not on your inactive tab

**ILC Hours**: Via this report, Managers and DTVs can now see in bulk the timesheet details by serial num and line item the ILC codes logged by ILC contractors including account id, work item id, activity code, and bill code

**Liability/Invoice Enhancement**: We have added Additional filtering capabilities for the existing Liability and Invoice Reports


<h3>7-7 Release</h3>

**New Timesheets Page**

We added a timesheets page allowing contractors to see a table of ALL of their timesheets, including saved (not submitted) timesheets and timesheets on multiple POs. This gives the contractor the ability to see the status of all of their submitted timesheets in a single view. This table can be downloaded and searched, it also shows the email of the manager, DTV and SAM who need to verify the timesheets.

**PO Cancellation**

This new function allows our application to process in a Purchase Order Cancellation from the upstream applications (Buy@IBM/Ariba). Once the PO has been cancelled, the Purchase Order and Contractor Record (if one was created prior to the cancellation) will be moved to the Cancelled tabs (Managers/CCA/FA/SAM). The Manager and the Supplier will receive an email notifying them that the PO was cancelled. We have created a function to allow timesheets on the cancelled PO to be migrated off of the Cancelled PO onto a renewal PO. This function is brand new so we highly recommend you read the training documentation in the PDF

For managers who are part of GBS or GTS, if the contractor admin teams move a PO or a contractor to their inactive tab, the PO or contractor record will also move this record for the assigned manager as well. This function helps keep the offboarding process more in sync and should help limit the automated reminder emails informing managers that the PO is running out of funds or the contractor records are expiring soon.

A new email will come out weekly to notify managers and DTVs when the have timesheets on their escalated tab. Since timesheet verification is an important weekly activity, we will be sending out weekly reminder emails for all timesheets which are escalated which means they have not been verified before the escalated deadline.


<h3>4/28 Release</h3>
Made it so that if there is a renewal PO that flows to the app and is linked in CSA to a PO already in the Blockchain Application with an "All Approved" contractor record, the contractor record on the new PO will automatically be created.


<h3>3/11 Release</h3>
Search function on Timesheets page enhanced to allow users to search by more fields Enabled ability to search by billing start date and billing end date on the Invoice Reconciliations page

Added the PO Start date and PO End date added to Purchase Orders bulk page table Enabled ability to SORT on the Purchase Orders bulk page (can sort by clicking on the column headers)

Removed "Manage ILC Accounts" option from the menu drop-down. This page is no longer used as contractors have ability to SEARCH and SELECT their valid ILC accounts

Delegated Time Verifiers will now have ability to migrate pending timesheets to the new/ renewal PO (ability previously held only by Managers)

Managers will now have a way to view, change, and delete scheduled DTV assignments on the new "DTV Schedule" page. This is for temporary DTV assignments, not permanent assignments.

New tab added to Purchase Orders page: "Pending Contractor Assignment"- this tab will show the new and renewal POs loaded to the application that do not yet have a contractor associated to them.

Contractor start and end date now pre-populated based on the information on the Purchase Order data in Ariba.

Timesheet enhancements for Contractors: Made it so that when a new timesheet is loaded, we will only copy over the valid timesheet rows from the previous weeks timesheet. For example If the ILC account claimed against this week expires at the end of this week, it will not be pre-populated to next weeks timesheet.

Timesheet rows will be marked as invalid if MANUALLY entered by user and NOT selected/validated. This will help with the "Invalid ILC Account" error before submitting timesheets. Only selected search entries will be valid entries able to be claimed against

More obvious Search button for searching ILC accounts

Added new function to allow users to clear out their ILC accounts for an entire line at a time

POs/ Contractors will now automatically move to "Inactive" tab for CCA and Mgr automatically after the 4-week grace period has passed

Enabled ability for admins to search by role or by email address on the Users page

We are continually trying to make your experienced more streamlined and enjoyable. Many of these enhancements came as a direct result from your feedback!
