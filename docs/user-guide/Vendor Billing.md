# Working With Vendor Billing

The Vendor Billing applications are primarily used to create invoices. Typically the transactional amounts accumulated by vendor deals are “imported” by vendor billing users who later “export” the invoiced amounts to Vendor Receivables for tracking and processing. Refer to the Vendor Receivables document for additional information.

# Editing The Vendor Receivable Address Book

The Work With Address Book application is used to add the distributor’s “remit to” address for the vendor billing invoices and alternative vendor addresses if needed.

1. Select option 10 (Vendor Receivables) from the Purchasing screen. The Vendor Relations screen appears.
2. Select option 2 (Vendor Billing) from the Vendor Relations screen. The Vendor Billing screen appears.
   - User: JEANNINE  Menu: VBCV1  Date: 9/21/22
3. Select option 3 (Work With Address Book) from the Vendor Billing screen. The Work with VR Address Book screen appears.
4. Press <F10> (Add New Entry). The Edit VR Address Entry Details screen appears.
5. Enter data for the following:
   - Name (35a) - company name of the distributor or vendor.
   - Address Line 1 (30a) - first line of the mailing address.
   - Address Line 2 (30a) - second line of the address.
   - Address Line 3 (30a) - third line of the address.
   - City (25a) - city of the mailing address.
   - State (2a) - state abbreviation of the address.
   - Zip Code (5n) - zip code of the address.
   - Zip Ext (5n) - 4-digit extension of the address.
6. Enter REMIT for the Address Type (6a) field if adding the distributor’s address.

# Adding An Invoice By Importing Vendor Deal Data

The instructions below describe using the Build Vendor Invoice application to create vendor billing invoices by importing data accumulated for vendor deals.

1. Select option 10 (Vendor Receivables) from the Purchasing screen. The Vendor Relations screen appears.
2. Select option 2 (Vendor Billing) from the Vendor Relations screen. The Vendor Billing screen appears.
3. To open the Build Vendor Invoice screen either select:
   - Option 2 (Build Vendor Invoice) from the Vendor Billing screen or
   - Option 1 (Work With Vendor Invoices) and press <F10> (Create Invoice) when the Work With Vendor Invoices screen appears.
4. Enter data for the following fields:
   - Optional: Vender # (6a) - the vendor code. If necessary press <F4> to select a vendor code from the Select Vendor Master screen.
   - Optional: Invoice Date (6n) - the invoice date.
   - Optional: Terms (3a) - a terms code. If necessary press <F4> to select a terms code from the Select Terms Description screen.
   - Optional: Due Date (6n) - the due date.
   - Import Deal # Activity (6n) - a vendor deal number. If necessary press <F4> to select a deal number from the Select Deal screen. The This is a mixed vendor deal. A separate invoice will created for each vendor message appears when a mixed vendor deal is selected.
   - Import Item Level Details for Deal? (1a) - Y (yes) to import item level information or N (no) to create a single line summary of the deal activity.
   - Include Items with Zero Accrual $ ? (1a) - Y (yes) to import item level information for items with no accumulated amounts.
   - Optional: Start Date and End Date (6n) - dates to limit the invoice to amounts accumulated during a designated date range.
5. Press <Enter> when data entry is complete.

# Adding A Vendor Billing Invoice Manually

The instructions below describe using the Build Vendor Invoice application to create a vendor billing invoice by entering the data manually.

1. Select option 10 (Vendor Receivables) from the Purchasing screen. The Vendor Relations screen appears.
2. Select option 2 (Vendor Billing) from the Vendor Relations screen. The Vendor Billing screen appears.
3. To open the Build Vendor Invoice screen either select:
   - Option 2 (Build Vendor Invoice) from the Vendor Billing screen or
   - Option 1 (Work With Vendor Invoices) and press <F10> (Create Invoice) when the Work With Vendor Invoices screen appears.
4. Enter data for the following fields:
   - Vendor # (6a) - the vendor code. If necessary press <F4> to select a vendor code from the Select Vendor Master screen.
   - Optional: Invoice Date (6n) - the invoice date.
   - Optional: Terms (3a) - a terms code. If necessary press <F4> to select a terms code from the Select Terms Description screen.
   - Optional: Due Date (6n) - the due date.
5. Press <Enter> when data entry is complete.
6. Press <F10> (Create Invoice) and press <Enter> when prompted to confirm.

# Printing Vendor Billing Invoices

The instructions below describe using the Work With Vendor Invoices application to print two versions of the vendor billing invoice. The first version uses a landscape format printed on “plain paper.” Version 2 is printed using the Formless Printing optional DAC module in a portrait format. Examples of both versions are included below. Contact CDR support personnel for additional information about the Formless Printing optional DAC module.

1. To print version 1 of the invoice locate the desired invoice in the screen’s list (use the restrictor fields or <Page Down> if necessary) and enter P (Print Invoice) in the selection column next to the vendor code and press <Enter>.
2. Enter N (no) and press <Enter> when the Would you like to email this Vendor Invoice? message appears.
3. Enter N (no) and press <Enter> when the Do You Want to Print a Separate Envelope Window Address Page? message appears.

# Exporting Invoice Data To Vendor Receivables

The instructions below describe using the Work With Vendor Invoices application to export invoiced amounts to Vendor Receivables for tracking and processing. Refer to the Vendor Receivables document for information about adding and applying vendor receivable transactions after the invoice data is exported.
