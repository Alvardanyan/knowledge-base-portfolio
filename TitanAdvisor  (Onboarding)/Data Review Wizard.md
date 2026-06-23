# Data Review Wizard

## Overview

Data Review Wizard helps ensure that the data imported to ServiceTitan is accurate. It streamlines the data validation process by resolving discrepancies and maintaining data integrity.

## Who uses this feature

- Administrators

- Primarily benefits Residential Service and Replacement, and Residential Construction business types

- Applies to all trades

## Feature configuration
- This feature is currently in Private Preview/Limited Release and is subject to change.

## Things to Know

- Data Review Wizard is for customers who are in onboarding.
- You will work with a Data Quality Analyst (DQA) to complete the data review process; the DQA will address all flagged items to ensure data readiness. The wizard is not meant to be completed independently and should only be completed with a DQA.
- The process focuses on reviewing data points for Customers, Invoices, Jobs, Estimates, and Equipment.
- After you finish the review, you won't be able to access Data Review again. The change is now in production and cannot be undone.
- Before finishing the data review process, you can reset the wizard by clicking Reset Data Review to restart the review from scratch.

> **Note:** Any changes applied before resetting the wizard will remain in the account if the data has not been wiped and reimported.

- All changes applied in the initial data review must be reapplied on the final import of data.

## View data dashboard

After importing the data into ServiceTitan, the Data Quality Analyst (DQA) shares their screen with you to start the review process and make fixes. The review process consists of three phases: High Level, Potential Issues, and Closer Look.
The dashboard view provides a high-level overview of captured data, To-dos, and completed data sets. For each phase of data entities, you need to review Customers, Invoices, Jobs, Estimates, and Equipment. The green checkmark shows that the entity is reviewed and approved. 
Each entity provides a graphical representation to visualize the numbers accordingly. 

## High Level overview

The High Level review is the initial phase of the data review process, where the focus is on verifying the overall totals of the imported data to ensure accuracy and consistency.

To start high level review:

1. Click Go to Next Step on the Data Dashboard screen.
2. On the Learn screen that opens, click Continue.
3. On the Confirm Total Customers screen, review the number of customers.

   a. If the general number of customers varies from the initial number of your customers, click No.

> **Note:** There is expected to be a slight discrepancy in the counts due to additional data being added to your source software after the initial pull. There may also be a discrepancy in the counts based on how ServiceTitan creates records when importing data from your specific source software.

   i. Select between Not enough records and Too many records.

   ii. Provide additional information to resolve the issue.

Do the total customers match what you expected? Yes No

Which of the following best describes the problem?

- Not enough records
- Too many records

Please provide additional information to help us resolve the problem.

b. If the general number of customers is mostly correct, click Yes.

> **Note:** For every entity, there are one or two questions with Yes and No answer options to identify the accuracy of the imported records and fix the data discrepancies.

4. Click Continue to move to the next entity. Repeat the same steps to reach the last entity.

## Review potential issues

The Potential Issues is the second phase of the data review process, where the focus is on verifying the common issues and applying bulk changes to fix them.

On every entity, you might find some items that are identified as potential issues.

You can also export the records as a CSV File.

To resolve the issues in bulk fixes, you can:

- Create a rule to fix them
- Leave the issue as is

### Create a rule

1. Click Create Rule to Fix.
2. Select a fix from the options.
3. When you're finished, click Apply Fix.

Select a fix and then build out your rule. Then, preview the results and apply the fix.

- Update Customer Name to be the street address
- Apply the "[Data Review - Missing Name]" tag to all customers

### Leave the issue as is

1. Click Leave Issue As Is.
2. On the Leave issue as is? popup, select Leave As Is.
3. The card will show as resolved.

> **Note:** After clicking Apply Fix or Leave Issue As Is, the action cannot be undone.

After completing potential issues, you are ready to move to the Closer Look phase.

## Take a closer look at data

Closer Look is the final phase of the Data Review process.

The focus is on analyzing the details of each imported entity to verify their accuracy and flag discrepancies.

To flag a discrepancy:

1. Click Flag to identify the incorrect data.
2. From the Specify what is wrong list, select the issue type.
3. In the text box that opens, enter the description of the issue.
4. When you’re finished, click Confirm and Continue.

> **Note:** You can flag as many data components as appear incorrect, however the text box is generic for all.

If you have any specific or high-profile customers whose information you want to review and ensure it looks correct:

1. Click Review Specific Customers.
2. On the Review Specific Customers sidebar.
3. Enter the name of the customer, and click Search.
4. Select the customer you want to review. 
5. When you're finished, click Add to Review.

This review and flag workflow is the same for the rest of the entities.

