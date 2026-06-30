# EOD Report — 09-06-2026
1. Created separate Google Sheets for therapists and case managers to capture Mandatory Outcome Measure data in a more structured and role-specific manner.
2. Developed a Google Apps Script to automatically push data from the main Mandatory Outcome Measure sheet into the respective therapist/case manager-specific sheets, reducing the need for manual data segregation.
3. Verified that the generated care team member sheets are being updated correctly from the parent sheet, including validation of the data mapping, sheet naming format, and overall data flow.
4. Set up the Outcome Measure workflow for production by creating the required care team member sheets, updating the parent sheet, configuring Google Cloud access for sheet permissions, and merging the updated codebase.
5. Deployed the Outcome Measure task to production and completed initial verification to confirm that the workflow is functioning as expected.

# EOD Report - 10-06-2026
1. Analyze the Nuview Outcome reports in the tableau and check what different data is shown there in the different dashboards.
2. Check the mezmo for error of Outcome measure and Analyze the issue of intake reminder job issue.
3. Fix the error of Intake reminder job and fix the incomplete outcome measure job for send wrong date of intake reminder forms.
4. Test the Outcome measure jobs and check now everything is working correctly or not.
5. Analyze the issue of wrong order of executions for the jobs and Research about any solution to run the consolidated email job at the last of the Mandatory outcome measure jobs.

# EOD Report - 11-06-2026
1. Find the solution for Wrong execution order of the Automated jobs in production server.
2. Check the Visitor Analytical API structure and started work on HubSpot Custom UI Card for Visitor Analytics.
3. Connect the Contact API and Visitor Analytics API with the card and map data into the UI components.
4. Adjust the UI components to handle the un-available data.
5. Added the error edge cases to handle the multiple cases including no tracking session id found, no tracking session found, API errors, etc,

# EOD Report - 12-06-2026
1. Test the wrong execution order of the Mandatory outcome measure jobs.
2. Deploy the Mandatory outcome measure jobs into the production server.
3. Check and verify the logs is everything seems correct or not, also check the Emails are sent correctly or not.
4. Added AC and Shalini into the CC recipient in the consolidated Outcome measure  emails.
5. Analyze the tableau dashboards and it's several reports, check it's data sources and it's linked fields.
6. Research about is it possible to use bastionGPT to create reports with the data.

# EOD Report - 15-06-2026
1. Check the different KIPU APIs and match the required data and fields in the demographics sheet.
2. Create a automated job to fetch the patients and their respective data from the KIPU APIs.
3. Create a method to map the demographic data into the required format to push it into CSV.
4. Check the KIPU patient evaluation APIs to get the data for the discharge client satisfaction survey.
5. Create a method to map the discharge client satisfaction survey into the required format for the CSV.
6. Test out the job, refactor the codebase and check the CSV format is correct as needed.

# EOD Report - 16-06-2026
1. Analyze the reports generate by the automated job and compare it with the actual reports.
2. implement the method to create a CSV sheet for patient's anticipated discharge date.
3. Verify the Job by running it and check is there any error in the job.
4. Analyze the Historical report sheet, check the main sources and understand how the report is being formed.
5. Verify the Evaluation APIs is sending total score in the response and in which format we are getting the score vales.
6. Implement the method to generate historical Outcomes report csv via KIPU APIs.

# EOD Report - 18-06-2026
1. Check the today's records which is enrolled with the session tracking from the website and Analyze the issues in the tracking session functionality.
2. Asked hemant to fix the issues in the website tracking issues.
3. Correct out the conversion summary incase of CTM call tracking and show the right conversion data in the conversion section.
4. Show the visited pages count, total event tracked counts and total time spent above every session.
5. Build a list of scenarios to test the website session tracking functionality and pass it to hemant for testing purpose. 
6. Show the UTM source and UTM campaign in front of every session.
7. Handle the edge case issues in the visitor tracking card and check works on different senarios.

# EOD Report - 19-06-2026
1. Analyze the issues that was fixed by the hemant and verify they are fixed in the staging environment.
2. Noted the persisted issues and assigned them to hemant for resolution.
3. Checked the Consolidated Mandatory outcome emails and verify does the patients are discharged or not.
4. Analyze the automated Mandatory outcome job and check why the discharged patients are being added into the emails and google sheet.
5. Fix the intake follow-up automated to prevent adding discharged patient into the upcoming assessment list.
6. Fix the intake follow-up job to get the care team from actual care-team API instead of hubspot evaluation process.
7. Test out the jobs and check does the job fixed for both issues or not.