# Physical Inventory

## Working With Physical Inventory

The Physical Inventory applications are used to compare and reconcile a count of the *entire physical inventory and all the on-hand quantities* of the DAC Item Balance files.

If a count of the entire physical inventory is not being done, refer to Adding An Inventory Batch of the Warehousing document for detailed instructions about using the Inventory Batch Entry application to do a cycle count inventory.

Refer to the DAC Default System Options document for information about the **Convert To Standard Sell**, **Variance Tolerance Qty** and **Variance Tolerance Value$** fields of the SYS038 (Physical Inventory Options) default system option.

>note: *The step-by-step instructions below 1) describe how to enter a minimum of one to a maximum of four counts of a warehouse's inventory, and 2) must be followed precisely in the order given.* As described below, any additional counts entered after the first count should be limited to only those items for which significant variances appear after entering the first count.

Read completely through these steps, and contact CDR support personnel if you have any questions *before* proceeding with the data entry described below.

**Step 1**: Verify that DAC is used to:

- Assign all items to locations.
- Post all customer invoices and credit memos.
- Receive all the purchase orders which have been received in the warehouse.
- Delete or post, as necessary, any existing inventory batches.
- Complete end of day processing. Note: End of week, end of period and end of year processing may be done before or after continuing the physical inventory.

**Step 2**: Print an Inventory Evaluation Report. It is recommended that you mark the report Before Inventory, and retain this report for accounting purposes. Refer to Printing Inventory Evaluation Reports below for additional information.

**Step 3**: Use one of the following to print count sheets if Cipher Lab or Telxon units are not used to enter the first inventory count:

- The Print Count Sheets application. Refer to Printing Physical Count Worksheets below for detailed instructions.
- The Cycle Count Sheets application. Refer to Printing Cycle Count Worksheets below for detailed instructions.
- A custom query count sheet report if available.

**Step 4**: Verify that all system users are signed on to DAC with different usernames, that no user has multiple sessions open, and that no individual user is signed on at more than one terminal with the same username.

**Step 5**: Use the Physical Inventory Guide application to place the system in Physical Inventory mode as describe below.

 Select option 4 (Inventory System) from the Main Operations Menu screen. The Inventory Menu screen appears.

 Select option 2 (Physical Inventory) from the Inventory Menu screen. The Physical Inventory Menu screen appears.

 Select option 3 (Physical Inventory Guide) from the Physical Inventory Menu screen. The Physical Inventory Guide screen appears.

 To place the system in Physical Inventory mode, enter a warehouse code for the Warehouse to take Physical Inventory on (6,a) field, and press &lt;Enter&gt;.

 When the Are you sure you wish to continue and place the system in Physical Inventory mode? message appears, enter Y for the OK? field (1,a) and press &lt;Enter&gt; to confirm. The Physical Inventory Menu screen appears with the The system is now in physical inventory mode message.

**Caution: Do not proceed with Step 6 until completing Step 5.** If users do not place the system in Physical Inventory mode, remote orders cannot be used to create inventory batches.

**Step 6**: Users who do not use Cipher Lab or Telxon units for physical inventory must skip this step and proceed with Step 9.

Use Cipher Lab or Telxon units to enter and transmit (send) the inventory counts as remote orders, but note the following:

- Before entering items and quantities, enter any number for the customer with a Cipher Lab unit or enter 000000 for the customer with a Telxon unit, and enter INVTRY for the route.
- The number of line items entered should be limited to 500.
- Important: Keep a record of the total number of remote orders entered and transmitted. This is required to later verify (as described in Step 7 below) that all the necessary inventory batches are created.

Refer to Working With Telxon of the Billing document for information about using Telxon units.

**Step 7**: Users who do not use Cipher Lab or Telxon units for physical inventory must skip this step and proceed with Step 9.

Users who use Cipher Lab or Telxon units must verify that all the necessary remote orders are transmitted and appear (with INVTRY as the route) on the Work With Remote Orders screen. If this is not done, the physical inventory will be incomplete.

Use the Work With Remote Orders screen to create an inventory batch from each transmitted remote order:

1. Enter *INVTRY* for the **Route** restrictor field and press &lt;Enter&gt;. The value of *INVTRY* will appear for both the **Routes From** and **To** fields under the Selection Criteria heading.

2. Press &lt;F5&gt; to mark the remote orders.

3. Press &lt;F10&gt; to process the marked orders.

    Refer to Working With Remote Orders of the Billing document for additional information.

After processing, each remote order will appear as an inventory batch record on the Work With Inventory Batch screen. Review the Remote Inventory Edit report for obvious errors in the inventory count.

Creating an inventory batch from each transmitted remote order as described above, will be done automatically by the system for some users. Refer to the DAC Default System Options document for information about the Transmission Placement field of the SYS033 (Billing Options) default system option.

**Step 8**: Users who do not use Cipher Lab or Telxon units for physical inventory must skip this step and proceed with Step 9.

Use the Work With Inventory Batches application 1) to correct the item counts of the inventory batches, and 2) to mark all the inventory batches for posting. Note: Users may choose to delay correcting item counts until after Step 10 when the physical count worksheets with variance data is printed.

  Select option 2 (Work With Physical Inventory Count Batches) from the Physical Inventory Menu screen. The Work With Inventory Batch screen appears.

  Enter 2 (Edit) in the selection column next to the desired batch, and press &lt;Enter&gt;. The Enter Inventory Counts screen appears.

 If necessary, change the control totals for the **Batch Quantity** and **Batch Count** fields.

 Press &lt;Enter&gt;. The Inventory Entry screen appears.

 If necessary, use *2=Edit Record* to correct an item’s count.  

 After verifying the accuracy of the total batch count and total batch quantity, enter these amounts for the **Count** and **Qty** fields, and press &lt;Enter&gt;.

 Press &lt;F10&gt; (Mark Batch For Post), and press &lt;F3&gt; (Exit). A Pending Transaction report is printed, and the Enter Inventory Counts screen appears.

 Press &lt;Enter&gt; when prompted to confirm. The Work With Inventory Batch screen appears.

 Repeat the previous steps until all the inventory batches are marked for posting, and press &lt;F3&gt; to exit. The Physical Inventory Menu screen appears.

**Important: Do not proceed until verifying that all the necessary inventory batches have appeared on the Work With Inventory Batch screen, and have been marked for posting.**

Select option 3 (Physical Inventory Guide) from the Physical Inventory Menu screen. The Physical Inventory Guide screen appears.

**Important: After completing Step 8, Cipher Lab and Telxon users must proceed to Step 10.**

**Step 9**: Use the Work With Inventory Batches application 1) to enter the first inventory count taken of the physical inventory if Cipher Lab or Telxon units **are not** used, or 2) to enter additional counts regardless of how the first count was entered.

Select option 2 (Work With Physical Inventory Count Batches) from the Physical Inventory Menu screen. The Work With Inventory Batch screen appears.

Press &lt;F10&gt; (Create Batch). The Enter Inventory Counts screen appears.

If desired, enter control totals for the Batch Quantity and Batch Count fields.

Press &lt;Enter&gt;. The Inventory Entry screen appears.

Enter data for the following fields to enter an inventory batch record for each counted item:

- **Item** (6,n) - the item number of the counted item. If necessary, press &lt;F4&gt; to select an item number from the Select Item By Description screen.
- **Qty** (7,n) - the item’s counted quantity. Users do not have to enter an inventory batch record for each item that has a 0 (zero) quantity.
- **U/M** (1,n) - the counted item’s unit of measure, or leave this field blank to use the item’s standard selling unit of measure.

 **Caution**: If a value is entered for the **U/M** field of an item, that value will appear as the default value of the **U/M** field for the next item, regardless of what the next item's standard selling unit may be. The system will only revert to using standard selling units when the user leaves the **U/M** field blank.

 >Note: If more than one inventory batch record is entered for the same item with the same unit of measure, the quantities will be added together.

 Press &lt;Enter&gt; when data entry for an item is complete.

 Continue entering an inventory entry batch record for each counted item.

 **Caution**: If a value is entered for the **U/M** field of an item, that value will appear as the default value of the **U/M** field for the next item, as illustrated above. The system will only revert to using standard selling units when the user leaves the **U/M** field blank.

 When data entry of the inventory batch is complete, press &lt;F10&gt; to calculate the total batch count and batch quantity.

 The total batch count and total batch quantity appear to the right of *Actual*, as illustrated above.

 If necessary, edit the inventory entry batch records to correct the totals by using C for the **Type** field, and changing the **Qty** fields of the necessary records.

 After verifying the accuracy of the total batch count and total batch quantity, enter these amounts for the **Count** and **Qty** fields, and press &lt;Enter&gt;.

 Press &lt;F10&gt; (Mark Batch For Post), and press &lt;F3&gt; (Exit). A Pending Transaction report is printed, and the Enter Inventory Counts screen appears.

 Press &lt;Enter&gt; when prompted to confirm. The Work With Inventory Batch screen appears.

 Repeat the previous steps to continue entering inventory batches for the current inventory count, or press &lt;F3&gt; to exit when all the batches for the current count are entered. The Physical Inventory Menu screen appears.

>Important: Do not proceed until verifying that all the necessary inventory batches for the current inventory count are entered and ready for posting.

    Select option 3 (Physical Inventory Guide) from the Physical Inventory Menu screen. The Physical Inventory Guide screen appears.

**Step 10**: When all the batches for the current inventory count are ready for posting, the Physical Inventory Guide application is used to print physical count worksheets with variance data, and to accept the inventory count before continuing with the physical inventory process.

To print the recount sheets with variance data, enter *1* for the **Accept current cycle, move to next** field, and press &lt;Enter&gt;.

When the This option accepts the counts from your current cycle, prints recount sheets with variances, and advances you to the next cycle message appears, enter Y for the **OK?** field (1,a) and press &lt;Enter&gt; to confirm.

When the *The previous cycle was accepted. You may now begin counting for the new cycle message*, press &lt;Enter&gt;. The Phyiscal Inventory Menu appears.

**Step 11**: If desired, use Step 9 and Step 10 to enter a second, third or fourth inventory count. Users are not required to enter more than one inventory count. After reviewing the variance data appearing on the physical count worksheets described above, users may continue the physical inventory process below without entering any other counts.

*Any additional counts entered after the first count should be limited to only those items for which significant variances appear after entering the first count.*

**Step 12**: The Physical Inventory Guide is next used to create a backup copy of the DAC Item Balance files, then update the on-hand quantities with the final count entered and accepted.

 Select option 3 (Physical Inventory Guide) from the Physical Inventory Menu screen. The Physical Inventory Guide screen appears.

 Enter 2 for the **Accept count** as-is field, and press &lt;Enter&gt;.

 When the This option will update your inventory with the counts from the cycles you have accepted message appears, enter Y for the OK? field (1,a) and press&lt;Enter&gt; to confirm.

 When the Should on-hand balances for uncounted items be set to zero? message appears, enter Y or N for the OK? field (1,a) and press &lt;Enter&gt; to confirm.

If Y is entered for the **OK?** field above, users have the option of clearing quantities of all uncounted items, or selecting uncounted items by warehouse area, pick region or location to clear quantities before continuing.

 When the Your live inventory has been updated with your accepted counts message appears, press &lt;Enter&gt; to confirm.

**Step 13**: Print an Inventory Evaluation Report. It is recommended that you mark the report After Inventory, and retain this report for accounting purposes. Refer to Printing Inventory Evaluation Reports below for additional information.

If after completing the steps described above, the user discovers that additional inventory counts must be entered, the Inventory Control application (option 1 of the Inventory Menu screen illustrated below) must be used, rather than the Physical Inventory application.

Refer to Working With Inventory Control of the Warehousing document for additional information.

If additional counts are entered, users should reprint the Inventory Evaluation Report as described in step 13 above.

## Printing Inventory Evaluation Reports

The Inventory Evaluation Report lists quantities on-hand for each unit of measure of
all the items.

1. Select option 6 (Reports Menu) from the Main Operations Menu screen. The
Reports screen appears.

1. Select option 5 (Inventory Reports) from the Reports screen. The Inventory
Reports screen appears.

1. Select option 1 (Inventory Evaluation Report) from the Inventory Reports screen.
The Inven. Evaluation Options screen appears.

1. Enter a warehouse code for the Enter Warehouse code (6,a) field. To change the
default value which appears, refer to Working With User Options of the Billing
File Maintenance document for information about the Default Warehouse field
of the user options records.

1. To use base cost for evaluating inventory, enter B (Base) for the Select Cost to be
used (1,a) field. If N (net) is entered, net cost is used for evaluating inventory.

1. Enter one of the following values for the Select Item Details (1,a) field to
desigante the level of detail appearing in the inventory evaluation report:
- Y - to print the report with an item level of detail.
- N - to print the report with a class level of detail.
- C - to print the report with a category level of detail. This value can be entered
only if option 1 is used (see Sort By Category, Sales Class, Descr. below).

1. To include stamp tax when evaluating inventory, enter Y (yes) for the Include
Home State Tax Stamps (1,a) field. This value can be entered only if option 1 is
used (see Sort By Category, Sales Class, Descr. below).

1. Enter 1 for one of the following fields to designate the sort method used to
generate the report:
- Sort By Category, Sales Class, Descr. (1,n) - to sort by category, sales class,
then by item description.
- Sort By Vendor Number (1,n) - to sort by vendor code.

1. If 1 is entered for the Sort By Category, Sales Class, Descr. field, enter data for
the following fields to limit the items appearing on the inventory evaluation report
by sales class:
- Beginning Class (5,n) - a sales class number. If necessary, press &lt;F4&gt; to
select a sales class number from the Select Sales Class Master screen.
- Ending Class (5,n) - a sales class number (or all 9s) must be entered. If
necessary, press &lt;F4&gt; to select a sales class number from the Select Sales
Class Master screen.

1.  If 1 is entered for the Sort By Vendor Number field, enter data for the following
fields to limit the items appearing on the inventory evaluation report by vendor:
- Beginning Vendor (6,a) - a vendor code. If necessary, press &lt;F4&gt; to select an
vendor code from the Select Vendor Master screen.
- Ending Vendor (6,a) - a vendor code (or all 9s) must be entered. If necessary,
press &lt;F4&gt; to select an vendor code from the Select Vendor Master screen.

1.  Press F6 (Print) when data entry is complete. The Inventory Reports screen
appears.

## Printing Physical Count Worksheets

The Print Count Sheets application is used to print the worksheets for handling a
physical inventory. As an alternative, the Cycle Count Sheets application can be
used to print worksheets that include the on-hand quantities in the item balance
records. Refer to Printing Cycle Count Worksheets in the Warehousing document for
additional information.

1. Select option 2 (Physical Inventory) from the Inventory Menu screen. The
Physical Inventory Menu screen appears.

1. Select option 1 (Print Count Sheets) from the Physical Inventory Menu screen.
The Prompt For Physical Count screen appears.

1. Enter a warehouse code for the Warehouse Code (6,a) field. Users may press
&lt;F4&gt; to select a warehouse code from the Select Warehouse Master screen.

1. To limit the items appearing on the Physical Count Worksheets by warehouse
area, enter data for the following fields before continuing with step 8:
- Beginning Area (6,a) and Ending Area (6,a) - a range of warehouse area
codes. Entering a value for the Beginning Area field is optional, but a valid
value (or all 9s) must be entered for the Ending Area field.
- End Location (9,a) - all 9s must be entered.

1. To limit the items appearing on the Physical Count Worksheets by pick region,
enter data for the following fields before continuing with step 8:
- Beginning Region (2,a) and Ending Region (2,a) - a range of pick region
codes. Users may press &lt;F4&gt; to select region codes from the Select Pick
Region File screen. Entering a value for the Beginning Region field is
optional, but a valid value (or all 9s) must be entered for the Ending Region
field.
- End Location (9,a) - all 9s must be entered.

1. To limit the items appearing on the Physical Count Worksheets by location, enter
data for the following fields before continuing with step 8:
- Beg. Location (9,a) and End Location (9,a) - a range of location codes.
Entering a value for the Beg. Location field is optional, but a valid value (or
all 9s) must be entered for the End Location field.
- Ending Region (2,a) or Ending Area (6,a) - all 9s must be entered for one of
these two fields.

1. To print the all the items of the warehouse, enter data for the following fields:
- End Location (9,a) - all 9s must be entered.
- Ending Region (2,a) or Ending Area (6,a) - all 9s must be entered for one of
these two fields.

1. To create a system-generated inventory batch for the items appearing on the
Physical Count Worksheet, enter Y for the Create Entry Batch? (1,a) field. Refer
to Working With Inventory Control of the Warehousing document for information
about using the Inventory Batch Entry application to work with inventory batch
records.

1. Enter one of the following values for the Location Type (1,n) field:
- 1 - Fixed pick
- 2 - Floating pick
- 3 - Fixed reserve
- 4 - Floating reserve
- 5 - Mixed regular
- 6 - Mixed damage.

 Note: The fields for which values are required to print Physical Count Worksheets
are Warehouse Code, End Location, Location Type, and either Ending Region
or Ending Area.

10. Press &lt;F6&gt; (Print). The Physical Inventory Menu screen appears.
