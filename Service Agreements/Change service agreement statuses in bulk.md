# Change service agreement statuses in bulk

## Overview
Perform bulk status changes to efficiently update multiple Service Agreements at once. Apply status adjustments to streamline renewal preparation, maintain workflow consistency, and organize agreements in bulk.

## Who uses this feature
* Administrators, accountants, project managers, and operations managers
* Primarily benefits Commercial Service and Replacement business types, and Residential Service and Replacement business types
* Applies to all trades

## Things to know
* You can apply a bulk status change to agreements that are in compatible lifecycle stages.
* Bulk status changes can be applied to agreements in Draft, Active, and Auto-Renew statuses.

## Change statuses in bulk
1. Go to the navigation bar and click Follow Up.
2. In the side menu, click Service Agreements.
3. From the Service Agreements page, select the agreements you want to apply a bulk status change to.
4. Click Actions, and from the dropdown select Change Statuses.
5. From the pop-up that opens, select the new status you want to apply:
   * Active: Activate draft or pending agreements.
   * Suspended: Temporarily pause active agreements.
   * Cancelled: Terminate active or auto-renew agreements.
6. In the Reason field, enter the reason for the change if required.

> **Tip:** Ensure all mandatory fields within individual agreements are filled out prior to attempting a bulk activation to prevent system processing errors.
>
> **Example:** If an agreement is missing a billing schedule, it will trigger an validation error during the status change.

7. Select the box for Send notification to customer if you want to automatically dispatch status update emails.
8. When finished, click Change Statuses.

## Change statuses in bulk (mixed agreement states)
When performing a bulk status change, additional configuration might be required if any of the selected agreements require specific approval permissions or have outstanding balances.

1. After you select the agreements and the target status, choose how to handle exceptions:
   a. Force status change and override blocks: This overrides minor system validation warnings and applies the status directly.
   b. Exclude agreements with validation errors: Keeps the problematic agreements in their current status while updating the rest of the batch. When this option is selected, additional summary options appear.
      * Log Errors
      * Notify Administrator
2. When finished, click Confirm Status Change.

## View status change errors
If the selected status adjustment cannot be applied to an agreement due to system constraints, the system stops the bulk action for that specific agreement and shows the error notification.

1. Click View Errors.
2. On the drawer that opens, view and fix the errors.
3. When finished, click Re-run Change Statuses.

Here are the error types and their descriptions:

| Error Type | Error Detail |
| :--- | :--- |
| Invalid Status Transition | Cannot move directly from Cancelled to Active status. |
| Skipped | Agreement must have a valid billing schedule configuration. |
| Missing Fields | Primary customer contact info is not set. |
| Permission Denied | User does not have authorization to approve status overrides. |

## Want to learn more?
* See Create a service agreement step 6: Finalize Status
* See Follow up on service agreements
