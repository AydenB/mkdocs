# User Guide: Receive Right

## Introduction

The Receive Right Module provides an interface to ProCat's Receive Right. This addition allows you to send orders from work with purchase orders to Receive Right. This user guide will walk you through the process of using Receive Right, from sending out purchase orders to receiving products.

## 1. Sending Purchase Orders to Receive Right

### 1.1 Accessing Receive Right Options

- Navigate to the "Work with Purchase Orders" section. 5, 1
- Look for the new option labeled "T=Rcv Right" on the top right side of your screen. This will be the option you will use to send the PO to Receive Right.

### 1.2 Sending a Purchase Order

- Once a purchase order is complete, add the "T" parameter in front of the purchase order number.
- Press enter, and a confirmation message will appear, indicating that the purchase order has been sent to Receive Right.

## 2. Checking Status and Batches

### 2.1 Monitoring Sent Purchase Orders

- To check the status, go to the "Work with RF Receiving" 5,8.
- Look for the option "F9 Receive Right Batches" to view all purchase orders sent to Receive Right.

### 2.2 Receiving and Updating

- Once the product is received and scanned by the recipients, the status will change to "C" for complete.
- Quantities and item counts will be displayed to confirm successful receipt.
- Use the standard process of putting "R" beside the purchase order to complete the receiving process. This will process the posting control report and edit lists like you are currently getting.

## 3. Handling Changes to Sent Purchase Orders

### 3.1 Editing Sent Purchase Orders

- If a PO was sent in error to Receive Right, you will need to remove the Receive Right batch and resend the PO.
- To remove the Receive Right batch. From Work With Receive Right Batches: 5, 8, &lt;F9&gt;, display the batch with 5, &lt;F3&gt;, &lt;F11&gt;, to be prompted to delete the batch. You can now resend the PO from Work With Purchase Orders option "T". This only applies before receiving the file.

### 3.2 Verifying Changes

- It is crucial to check with Procat to confirm that editing and resending a purchase order will not disrupt the process on the Receive Right side.

## 4. Testing and Training

### 4.1 Internal Testing

- Consider testing the Receive Right process internally using a test purchase order.  
- Send it through the system but cancel the receiving part (DO NOT USE R TO RECEIVE) to avoid affecting actual inventory.
- Plan a full-circle test with a small vendor to ensure a smooth process from sending to receiving.

### 4.2 Timing Considerations

- Discuss the best timing for sending purchase orders to Receive Right with the purchasing team.
- Consider sending them at the end of each night for efficient processing.

## FAQ
Automatically closing Back Orders is in development
    
Partials orders will need to be edited to fix the qty of the order to match qty shipped
    
To delete a PO batch, use a 5 to get into the batch. Press enter until you get to the display scan details. From there you can &lt;F11&gt; to delete. 
