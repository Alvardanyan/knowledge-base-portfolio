# HubSpot integration overview in Convex

## Overview

Transfer key business information from Convex to HubSpot to ensure your HubSpot environment
stays up to date, saving you time and minimizing manual data entry.

## Who uses this feature

* Managers, regional managers, representatives, and salespeople
* Primarily for Commercial Service and Commercial Construction business types

## Feature configuration

* Contact [marketing@convexlabs.io](mailto:marketing@convexlabs.io) to set up a demo and get more information about Convex.

## Things to know

- To setup an integration between Atlas and your CRM platform, generate API credentials for
HubSpot and share them with your Customer Success Manager (CSM). Your CSM will help
you set up the integration and customize data mappings to fit your business needs.

- Atlas sends relevant information, such as the company details, property addresses, and
contact information, directly into HubSpot.

## Push to CRM

Push to CRM is a feature in Atlas that allows you to manually trigger the sync of selected
property and contact data into your HubSpot.

1. Go to the navigation menu and click Map, then select a property.

2. From the Properties details panel (PDP) that opens, click Push to CRM.

The integration sends the following information:

- Property details: Company name, address, and any other associated custom fields.

- Contact details: Names, phone numbers, emails, titles, and social profiles.

> **Note:** Make sure to associate a contact with a property if you want to send contact
information to HubSpot.

# HubSpot Objects

Integration creates the following HubSpot Objects:

- Create Company: If enabled, the workflow:
  - Creates or updates a Company in HubSpot.
  - Checks HubSpot to avoid creating duplicate records.
  - Company ownership is assigned using the account owner's email from Atlas.
  - The HubSpot Company is linked back to the property in Atlas.

- Create Contacts: If enabled, the workflow:
  - Checks if the Atlas contact is already linked to a HubSpot contact.
  - Updates existing contacts or creates new ones if needed.
  - Links contacts to the associated Company in HubSpot.

- Create Deal: The workflow:
  - Creates a Deal in HubSpot and links it to the appropriate Company.

| Term | Definition |
| --- | --- |
| Contact (HubSpot) | A business or organization in HubSpot. Often represents the customer account and can be linked to multiple Contacts and Deals. |
| Company (HubSpot) | A business or organization in HubSpot. Often represents the customer account and can be linked to multiple Contacts and Deals. |
| Deal (HubSpot) | A sales opportunity or transaction tracked in HubSpot. |

## Sync HubSpot Data to Convex

This workflow is used to populate Atlas with existing CRM data from HubSpot. It usually runs a
single time during setup to show relevant HubSpot Companies in Atlas.

#### Workflow Behavior:

1. Query Accounts from HubSpot: Retrieves all HubSpot Companies created since the last
time the workflow ran.

2. Match Companies to Properties in Atlas: For each HubSpot Company, the workflow checks
for an existing link to a Convex Property using the CRM ID.

> **Note:** CRM ID is a unique identifier for a Company or Contact in HubSpot that Atlas uses
to match or link records during syncing.

a. If no CRM ID match is found, it attempts to match the property by address.

b. If a match is found, it proceeds to enrich the Property with Company data.

3. Update Property Record in Atlas: The matched Atlas Property is updated with the data
from the HubSpot Company.

4. Sync Company Contacts: If enabled, this workflow:

a. Retrieves contacts linked to each HubSpot Company.

b. Compares with existing Atlas contacts.

c. Updates whichever version is older.

d. Creates and links new contacts in Atlas if they don't already exist.

## Want to learn more?

- See Salesforce integration overview in Convex

- See Pipedrive integration overview in Convex
  
