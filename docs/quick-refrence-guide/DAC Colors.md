# DAC Colors
## Accounts Receivable
### Display Customers for A/R
DSQXDFR (2,3)  
<span style="background-color:green">**GREEN**</span>  Customer name - Customer has notes.  
 <span style="background-color:green">**GREEN**</span> Y in Note column - Customer has notes.
### Display A/R For Inquiry
DSF0DFR (2,2,5 and 2,3,5)  
<span style="background-color:green">**GREEN**</span> I under T column - Invoice type order has excluded commissions.

## Billing
### Work with Items
HWJ4DFR (1,2,1)  
<span style="background-color:red">**RED**</span> Date- last sold date over 1 year

### Work With Orders
DSJWDFR (3,1)  
 <span style="background-color:blue">**BLUE**</span> Order source - Order has a message: I = Internal (Pick slip) / D = Delivery (Driver Manifest v. C).  
<span style="background-color:green">**GREEN**</span> Order number - Order is a Credit Memo order type.  
<span style="background-color:red">**RED**</span> Order status - Order is locked, and usually indicates someone is editing the order.  
 <span style="background-color:yellow">**YELLOW**</span> P order type - More than two days have passed since the order was picked.

### Order Entry
 GSSADFR (3,1,F10 and 3,1,2)  
<span style="background-color:green">**GREEN**</span> Order quantity - Quantity ordered is greater than quantity shipped.  
<span style="background-color:red">**RED**</span> Price below base cost

### Work With Load Control
BSRXDFR (3,19,1)  
<span style="background-color:red">**RED**</span> Invoice number and Pick region - Indicates the transaction has not been marked or changed.

## Purchasing
### Work With Vendors
 DSI8DFR (5,2)  
 <span style="background-color:white">**WHITE**</span>
 Vendor name - Vendor has notes.

### Work With Vendor Items
 DSJBDFR [or Vendor Items: DMGUDFR] (5,2,5)  
 <span style="background-color:green">**GREEN**</span> Item description - Buying allowance or VR purchasing deal exist. [ all types of VR pur deals?]  
 <span style="background-color:green">**GREEN**</span> Available quantity [AVBL or AVAIL] - Item is on order.  
 <span style="background-color:white">**WHITE**</span> Item number - Seasonal warning / [is?] approaching. [ DMGUDFR only? ]  
 <span style="background-color:white">**WHITE**</span> Forecast average [Forcst Avg or FCast Ave] - Seasonal information is available for the item.  
 <span style="background-color:yellow">**YELLOW**</span>
 P below ? field [or between X and SOQ columns] - Pre-book order exists for the item.  
 <span style="background-color:yellow">**YELLOW**</span>
 N after Dys ROP column [or between SOQ and ROP columns] - New item (45 days or less).

### Explode Vendor/Items Details
DSJ8DFR (5,2,5,5)  
 <span style="background-color:blue">**BLUE**</span>
 F on same line as OQ$ and to far right - Future [buying] allowance is found for the item. [no longer used * ]  
 <span style="background-color:green">**GREEN**</span>
 On order quantity - PO is past expected date or scheduled date.  
 <span style="background-color:green">**GREEN**</span>
 OQ Cases - Always highlighted, but only populated if SOQ exists.  
 <span style="background-color:red">**RED**</span> Deal description - [ More than one ] buying allowance or VR purchasing deal exist.  
 <span style="background-color:white">**WHITE**</span>
 Quantity after Lost Qty Last Week - Quanity of lost sales for the item last week. [ not Green ]  
 <span style="background-color:white">**WHITE**</span>
 Net cost - Indicates it is used to calculate cost for POs.  
 White Mfr. list - Indicates it is used to calculate cost for POs.  
 <span style="background-color:yellow">**YELLOW**</span>
 S highlighted in yellow and after O/I SELL? - Item selling allowance exists.  
 <span style="background-color:yellow">**YELLOW**</span>
 V highlighted in yellow and after O/I SELL? - VR purchasing deal exists.  
 <span style="background-color:yellow">**YELLOW**</span>
 B highlighted in yellow and after O/I SELL? - Item selling allowance and VR purchasing deal both exist.

### Work With Purchase Orders
BSDSDFR (5,1)  
 <span style="background-color:pink"> **PINK** </span>
 Expected date - PO is past expected or scheduled date.  
 <span style="background-color:white">**WHITE**</span>
 Vendor number - Back Haul Status of PO header is Y.  
 <span style="background-color:yellow">**YELLOW**</span>
 B in BO column - Backorder PO exists.

## MISC
### ACH Batches
DPHGDFR (11, 12)  
<span style="background-color:red">**RED**</span> Amount - partial apply amount

### Display Delivery Routes
(1,5,7)  
<span style="background-color:red">**RED**</span> Customer Name- Delivery route inactive

### Work With Contracts
(1,3,1,5)  
<span style="background-color:red">**RED**</span> Conract Value- if 0%

### Work with Pre-Book Orders
(3,22,19,1,C)  
<span style="background-color:red">**RED**</span> Customer- inactive
