# Enable Auto-renew for Service Agreements

## Overview

Auto-renew allows you to automatically generate a new service agreement before the current one expires, enabling your team to activate it without starting from scratch. This keeps coverage continuous and reduces the manual work of tracking and renewing agreements individually.

## Things to know

- Auto-renew generates a new agreement in Auto-renew status 90 days before the End Date of the current agreement. The current agreement doesn't extend, and it stays active until its end date.
- If you enable Auto-renew while the agreement is already inside the 90-day window, the renewal copy is created immediately.
- The auto-renewed agreement sets the Start Date to the day after the current agreement's End Date. The system copies the scope-relevant data, such as Locations, Visits (with visit windows recalculated for the new term), Equipment, and Tags.
- You still need to activate the auto-renewal and complete any required e-signatures before it goes live.
- If you disable auto-renew while a next-term record is still in Auto-renew status, the system removes that record. If the next term has already moved past Auto-renew status, disabling auto-renew does not remove it.

## Who uses this feature

- Administrators and CSRs
- Primarily benefits Commercial Service and Replacement business types, and Residential Service and Replacement business types
- Applies to all trades

## Feature configuration

- Account configuration is required to use this feature. Please contact Technical Support for details.

## Use Case

Many contractors offer "ongoing" or "perpetual" service agreements, where the same scope of work repeats year after year until one party chooses to cancel. These agreements often include annual pricing reviews or increases.

In ServiceTitan, all Service Agreements require an end date and cannot be configured as truly open-ended agreements. To best model perpetual agreements, ServiceTitan recommends creating agreements with:

- A 1-year term and Auto-renew enabled.

With this setup, the agreement automatically renews each year without requiring manual effort. This approach also provides several operational and accounting benefits, including:

- Simplified annual price adjustments through bulk pricing updates.
- Clear agreement periods for reporting and auditing.
- Better isolation of accounting or deferred revenue issues to a single agreement term.

Because each renewal creates a new agreement term, any accounting or data discrepancies are contained within that specific period rather than carrying forward indefinitely. This makes reconciliation, auditing, and issue resolution significantly easier.

Example:

Rather than creating a 20-year agreement to represent a "perpetual" customer relationship, the recommended approach is to create a 1-year agreement with Auto-renew enabled. This more accurately reflects how perpetual agreements are managed operationally while taking full advantage of ServiceTitan's renewal and pricing workflows.

## Set a Default Auto-renew on Service Agreement Template

1. Go to the top toolbar and click Settings.

2. In the side panel, go to Operations > Service Agreement Templates.

3. Click Edit next to the template you want to update.

4. In the Default Values section, find Auto-renew and select Enabled.

5. When finished, click Save.

![image alt](https://github.com/Alvardanyan/knowledge-base-portfolio/blob/2c879021e31a4e4333b9d4bb507fb1be7e2dec7a/images/auto-renew-service-agreements-image-8b9bza5n.jpg)

> **Note:** This setting applies only to new agreements, and it does not change existing ones.

## Enable Auto-renew per Service Agreement

### Activate Auto-renew During Agreement Creation

1. In the agreement creation workflow, go to Step 4: Scope of Work.

2. Click Edit next to Auto-renew and from the pop-up select Enable Auto-renew.

![image alt](https://github.com/Alvardanyan/knowledge-base-portfolio/blob/1ebd8d49ffa3cb1bbbf5641afe6d4cc9cbfb3ed9/images/auto-renew-service-agreements-image-qhnbaqz9.jpg)

> **Note:** The default state of the Auto-renew comes from the service agreement template.

3. When finished, click Save Changes.

Continue completing the remaining steps to finish creating the agreement.

### Activate Auto-renew on an Active Agreement

1. Click an active service agreement to open the Service Agreement Management view.

2. Click Edit next to Auto-renew and from the pop-up select Enabled.

![image alt](https://github.com/Alvardanyan/knowledge-base-portfolio/blob/06553c99fe2cf29289dff5447b1c0223bccd2e92/images/auto-renew-service-agreements-image-3gjb6pp4.jpg)

3. Click Update Setting, and then click Enable Auto-renew.

> **Tip:** To view the renewal history for an agreement, click View History. Then click the Agreement ID to open that renewal version.

## Billing Schedule for Renew / Auto-renew Agreements

When a service agreement renews, its billing schedule carries forward based on how your current agreement schedule is configured. There are three scenarios:

- Default schedule, no changes: If your current agreement uses one of the default billing schedules (Time of Service, Upfront, Annual, Biannual, Quarterly, or Every Other Month) and you haven't modified it, the renewal agreement will automatically use that same schedule. Example: Current schedule → Quarterly (no changes) | Renewal schedule → Quarterly.
  
![image alt](https://github.com/Alvardanyan/knowledge-base-portfolio/blob/ff6fd1ce86d1afd67720c8b38a9d42f9f40e14c7/images/auto-renew-service-agreements-image-j41r5r8h.jpg)

- Default schedule, with modifications: If your current agreement uses a default billing schedule but you have made changes to it (such as adding or removing invoices or adjusting billed amounts), the renewal agreement will revert to the original default schedule, not your modified version. Example: Current schedule → Quarterly, with the fourth invoice removed and the third invoice doubled in price | Renewal schedule → Quarterly, restored to 4 equal invoices at equal intervals.

![image alt](https://github.com/Alvardanyan/knowledge-base-portfolio/blob/14ee9c89259d376d0e59c6e1ae2a1c81f661fd46/images/auto-renew-service-agreements-image-kpt5l0a0.jpg)

- Custom schedule: If your current agreement uses a custom billing schedule, the renewal will carry forward that same custom schedule. Example: Current schedule → Custom | Renewal schedule → Custom.

The system automatically recalculates all dates to align with the renewal, so no manual date adjustments are needed.

## Want to Learn More?

- See Renew Service Agreements in bulk
- See Service Agreement Management overview
