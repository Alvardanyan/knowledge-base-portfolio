# Set up deferred revenue for service agreements

## Overview

Use deferred revenue to recognize a portion of service agreement income as services are provided. In a given month, recognized revenue offsets the cost of providing these services, which can help you manage cash flow and profitability.

## Who uses this feature

• Administrators and CSRs

• Primarily benefits Commercial Service and Replacement business types, and Residential Service and Replacement business types

• Applies to all trades

## Feature configuration

• Account configuration is required to use this feature. Please contact Technical Support for details.

## What is deferred revenue?

Deferred revenue is used in accrual accounting to manage advanced payments for upcoming services. After accepting payment, you only recognize it as income upon delivery of services, when the revenue is earned, or it is spread out evenly over the months of the service agreement's active period.

For example, a service agreement where the customer pays upfront might include 4 quarterly maintenance visits. With deferred revenue:

• The upfront billing of the service agreement is deferred, increasing the liability General Ledger (GL) account balance.

• Every time a visit is completed, the invoice debits the revenue from the liability account and credits it into the income account.

## Set up service agreement templates for deferred revenue

With deferred revenue, revenue is routed into a liability general ledger account as money is invoiced. Then, as services are delivered or based on straight-line monthly recognition, revenue is moved into an income GL account.

There are two options for deferred revenue recognition:

• Percent-complete: The revenue is recognized proportionally based on the progress of work completed during each visit.

• Straight-line: The revenue is recognized evenly across the monthly periods within the duration of an agreement.

Both types require different setups. Follow the steps below to create the right deferred revenue recognition for your business.

## Percent-complete

Deferred revenue based on percent complete is used in accrual accounting to manage advanced billing for upcoming services. After billing, you recognize it as income upon delivery of services, when the revenue is earned.

Follow these steps to set up deferred revenue for Percent-Complete:

### Step 1. Set up your General Ledger accounts

Set up a GL liability account for service agreement revenue and a GL income account for recognized service agreement revenue in QuickBooks:

• Set up general ledger accounts

• QuickBooks Desktop: QBD Onboarding Step 1: Set up QuickBooks General Ledger Accounts (QBD)

• QuickBooks Online: QBO Onboarding Step 2: Set up GL accounts in QuickBooks Online

You can also map service agreement-related service items in your pricebook to Item GL Groups in Intacct:

• Map Pricebook items to Intacct Item GL groups

### Step 2. Create Pricebook service items for deferred revenue

You'll need to set up one item (negative liability pricebook service) that debits deferred revenue from the GL liability account and then set up another item (positive income pricebook service) that credits the revenue in the GL income account. Follow these steps:

• Create Pricebook service items for deferred revenue

#### Use case of Percent-Complete Calculation

To calculate the amount of revenue to recognize on a visit, ServiceTitan uses the Labor (including Extra Travel Time) and Material Costs Estimates for that visit and calculates that visit's contribution to the Total Cost. That contribution percentage is multiplied by the Total Agreement, see below:

Visit Cost Contribution % = Visit Cost / Total Cost

Visit Recognition Amount = Visit Cost Contribution % × Total Agreement Price

Example:

• 2 Visits

• Visit 1 Cost Estimate = $300

• Visit 2 Cost Estimate = $100

• Total Agreement Price = $500

VISIT 1:

Visit 1 Cost Contribution % = (Visit Cost) / (Total Cost) = $300 / $400 = 0.75

Visit 1 Recognition Amount = 0.75 × $500 => Visit 1 Recognition Amount = $375

VISIT 2:

Visit 2 Recognition Amount = 0.25 × $500 => Visit 2 Recognition Amount = $125

TOTAL:

Total Recognition Amount = $375 + $125 = $500

Total Recognition Amount = Total Agreement Price

> **Note:** If you don't see this option available in your account, please contact Technical Support or your Success Manager for details.

## Straight-line

Straight-line revenue recognition is an accrual accounting method that schedules regular revenue postings over the agreement's lifetime. After an agreement is activated, revenue is spread over the lifetime of the agreement, and income is posted evenly month over month.

Unlike percent complete revenue recognition, you do not need to select or create a Pricebook service item to recognize revenue. Instead, you can choose the income general ledger account on which the revenue is recognized over the lifetime of the active service agreement, independent of the items on the invoice.

Follow these steps to set up deferred revenue for Straight-line:

### Set up your liability and income General Ledger accounts

You need to set up a liability general ledger account and an income general ledger account in ServiceTitan along with a GL income account for recognized service agreement revenue in QuickBooks and in ServiceTitan:

• Set up general ledger accounts

• QuickBooks Desktop: QBD Onboarding Step 1: Set up QuickBooks General Ledger Accounts (QBD)

• QuickBooks Online: QBO Onboarding Step 2: Set up GL accounts in QuickBooks Online

After the GL accounts are set up for liability and income accounts in your accounting software and are mapped accordingly with the general ledger accounts set up in ServiceTitan, an invoice is generated at the end of every month to recognize the revenue.

# Want to learn more?

• Service Agreements - FAQ
