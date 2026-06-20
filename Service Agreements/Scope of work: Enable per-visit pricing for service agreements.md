# Scope of work: Enable per-visit pricing for service agreements

## Overview

Use per-visit pricing to define a clear dollar amount for each visit within a Service Agreement. This gives you flexibility to match billing to actual service delivery, especially when visit values vary. It provides clear billing and transparency to customers regarding visit-specific charges, and reduces misunderstandings. You can present a per-visit pricing breakdown, $150 per visit for 8 visits, making agreements easier to approve and manage.

## Things to know

- After the Per-Visit Pricing is enabled on a Service Agreement, the Total Agreement Price cannot be changed after the agreement is activated.
- To update the per-visit price or the Total Agreement Price on an active agreement, you need to disable the per-visit pricing feature.
- If the agreement has a recurring billing schedule, per-visit pricing allows you to control the amount of revenue that is recognized by each visit.

## Who uses this feature

- Administrators, accountants, estimators, project managers, and operations managers.
- Primarily benefits Commercial Service and Replacement business types.
- Applies to all trades.

## Enable Per-visit price

Enabling the Per-visit Pricing you can set the price for each individual visit, and the Total Agreement Price is calculated as the sum of all visit prices.

1. In the Service agreement creation process, when you reach the Scope of work step, click the **Enable per-visit pricing** box to enable the feature.
2. After you complete all the details in this step, click **Continue** to start adding visits to the agreement.

## Add visits and their prices

> **Note:** After activating the agreement, a Visit Price column appears in the visit table, allowing you to see the amount assigned to each visit.

1. In the Scope of Work screen, click **+Add Visit** to add the desired visits to the agreement.
2. In the Add Visit screen that opens, enter the following visit details:
   a. **Visit Name:** Enter a name for the visit.  
   b. **Visit Recurrence:** Select **Repeat** to make the visits recurring or select **Do not repeat** for a one-time visit. For more details on visits types, see *Visit Recurrence and step 4: Scope of work*.
3. **Visit Window / Visit Window Length:** Set the duration of the visit windows for all visits created through this recurring visit. The Visit Window for each individual visit can be modified after the series is created.
4. **Visit Price:** Enter the amount you want to charge the customer for each service visit included in the agreement. The Total Agreement Price automatically calculates the total based on the number of visits and the price per visit.

> **Note:** If you select the Visit Recurrence as Repeat, the Visit Window cannot be edited. Instead, the Visit Window Length field appears. This sets the duration of the visit window for all visits created through the recurring setup. The visit window for each individual visit can be modified after the recurrence is set up.

> **Note:** If you create a Quarterly recurring visit for an agreement with a duration of 12 months, the agreement will have 4 total visits. If the per-visit price is set to $1000, the Total Agreement Price will be the sum of all visit prices $1000 * 4 = $4000.

5. Make sure to fill out the rest of the required information for the visit and click **Save**. For more information, see *Create a service agreement step 4: Scope of work*.

## Configure Billing Schedule

The Per-Visit Price feature is compatible with all existing billing schedules offered for Service Agreements. Setting prices per visit ensures invoice totals match your expectations, especially useful for seasonal or uneven visit values. There are a few differences between the following billing options:

- **Time of Service:** When enabled, each visit that is booked in a job, the job invoice reflects the price set for that specific visit.
- **Recurring Billing:** The total agreement price is divided across the billing periods unless billing per visit is explicitly configured.

## Edit total agreement price on active agreement

The Agreement Price becomes locked and read-only, reflecting the total sum of all visit prices. To edit total agreement price on active agreement:

1. Edit the prices for individual visits.
   a. Go to the **Visits** section.
   b. Click the **Actions** dropdown and select **Edit Visit**.
   c. Update the **Visit Price**.
   d. Click **Save** to update the price. The price update also reflects on the Total Agreement Price.

2. Disable per-visit pricing to manually set the total agreement price.
   a. From the active agreement page, click **More**.
   b. Click **Disable Per-visit Pricing**.
   c. On the newly opened window click **Disable**.
   d. To update the Total Agreement Price, from the active agreement page, click **More**.

> **Warning:** Disabling per-visit pricing cannot be undone. This permanently removes all per-visit prices and recalculates visit revenue for unscheduled visits. The system automatically distributes the Total Agreement Price on all remaining unscheduled visits.

   e. Click **Edit Total Agreement Price**.
   f. Update the **Total Agreement Price** and click **Save**.

## Want to learn more?

- See Create a new document template with Template Manager
- See Create a service agreement step 7: Preview and Send
