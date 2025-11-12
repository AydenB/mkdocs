# User Guide: Count Right

## Introduction

The Count Right Modules provides an interface to Procat's Count Right- https://www.procatdt.com/solutions/countright . This addition allows you to leverage the Count Right system for managing your inventory cycle count sheets. 

## Creating an Inventory batch
You will need to create an inventory batch to be sent over to Count Right. From the main menu navigate to Cycle Count Sheets: 4, 1, 21, 3. From here you will create count sheets based on the area, location, or region. You will want to set Create Entry Batch to Y as well as set the option to Print on Hand qty. Once your selection is made, press &lt;F6&gt; to print. This will create a cycle count sheet in WRKSPLF as well as create a new batch in Inventory Batch Entry. 

## Sending to Count Right
Now that the inventory batch has been created and the cycle count sheet has printed, you will navigate to inventory Batch Entry: 4, 1, 1. From here you will see your recently created batch. You will now need to select that batch with the "T" option to send this batch to Count Right via folder IVCNTOUT. Now that the file is available for Count Right, you will then use the hand held to complete the process of counting. This batch will be locked and highlighted red until the hand held sends back the file. 

## Posting the count sheet
Once the user has completed their count and released the file back to DAC. You will resume posting the cycle count as normal. Navigate to the Inventory Batch Entry menu: 4, 1, 1. Use a 2 to edit the batch, and then &lt;F10&gt; to post the batch. 

## FAQ
Most errors are caused from Cycle Count batch not being created through 4, 1,21, 3, but through 4, 1, 1. Reviewing the BSIZPFR$ or GSK9PFR$ will show the transaction type as 'A'. This is incorrect and should be 'C'.
![alt text](../images/CR_CycleCountError.png)