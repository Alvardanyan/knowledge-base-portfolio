# Change prices in bulk for service agreements

## Overview
Perform bulk price changes to efficiently update multiple Service Agreements at once. Apply flat or percentage-based price adjustments and perform key bulk edits to streamline renewal preparation, maintain pricing consistency, and protect margins.

## Who uses this feature
* Administrators, accountants, project managers, and operations managers
* Primarily benefits Commercial Service and Replacement business types, and Residential Service and Replacement business types
* Applies to all trades

## Things to know
* You can apply a bulk price change to agreements that have the Total Agreement Price set.
* Bulk price change can be applied to agreements in Draft and Auto-Renew statuses.

## Change prices in bulk
1. Go to the navigation bar and click Follow Up.
2. In the side menu, click Service Agreements.
3. From the Service Agreements page, select the agreements you want to apply a bulk price change to.
4. Click Actions, and from the dropdown select Change Prices.
5. From the pop-up that opens, select how you want to apply the change:
   * $ (Flat amount): Adjust the agreement price by a fixed dollar value.
   * % (Percentage-based): Adjust the agreement price by a percentage of the current total.
6. In the Price Adjustment field, enter the value for the change.

> **Tip:** If you want to increase the price, set a positive value. To decrease the price, add a negative value.
>
> **Example:** Entering -3 in percentage decreases the agreement price by 3%.

7. Select the box for Round to the nearest dollar to round up the new calculated price to the nearest whole dollar amount.
8. When finished, click Increase Prices or Decrease Prices depending on the value you set.

## Change prices in bulk (mixed pricing modes)
When performing a bulk price change, additional configuration might be required if any of the selected agreements use the Markup Value and Surcharge pricing mode.

1. After you select the agreements and the price value, choose how to update the pricing:
   a. Apply the same $ and % change as above: This switches the selected agreements from Markup and Surcharge to manually defined pricing.
   b. Update markup value and surcharge instead: Keeps the selected agreements in Markup and Surcharge pricing mode. When this option is selected, additional fields appear. At least one of these fields must be set.
      * Labor Markup
      * Labor Surcharge
      * Material Markup
      * Material Surcharge
2. When finished, click Change Prices.

## View change price errors
If the entered price adjustment would cause any selected agreement's Total Agreement Price to become less than or equal to $0, the system stops the bulk action and shows the error notification.

1. Click View Errors.
2. On the drawer that opens, view and fix the errors.
3. When finished, click Re-run Change Prices.

Here are the error types and their descriptions:

| Error Type | Error Detail |
| :--- | :--- |
| Invalid Price | Total agreement price can't be negative. |
| Skipped | Agreement must be in one of these statuses: Draft, Sent, Rejected, Accepted, or Auto-renew. |
| Missing Fields | Total Agreement Price is not set. |
| Missing Fields | Some visits do not have a visit price set. |

## Want to learn more?
* See Create a service agreement step 5: Pricing
* See Follow up on service agreements
