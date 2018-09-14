# BOM_reconciliation
Description of Macro: 
This macro takes two BOMs and can identify any differences between them.  It will put changes in red font to the quantities, lengths, or both.  It will also identify any items removed from the old BOM with strikethrough font and new items added to the new BOM with the whole line in red font.

Steps to run:
0. *Sheets must be formatted as Columns A-E in the order:
 Item | Size | Description | Length | Quantity  | Unit

1. Clear the contents of both sheets "oldBOM" and "newBOM" using the two buttons above titled: "Clear oldBOM" and "Clear newBOM"
2. Paste the old BOM into the sheet "oldBOM"
3. Paste the new BOM into the sheet "newBOM"
4. Optional: Clear existing formatting on both BOMs using the button "Clear sheet formatting"
5. Click the button "Run BOM Comparison Macro"

Results: 
A. oldBOM
- Materials that were changed will have font color red
- Materials that were removed entirely will have font strikethrough

B. newBOM
- Materials that were changed will have font color red
- If the entire column is red, it is a new item to the BOM

C. genBOM
This tab is a new generated BOM that should be the final product.  It will be:
- The oldBOM, formatted with changes to QTY/Lengths in red
- Any items removed and red, strikethrough, and QTY = 0
- Any items new to the newBOM are added at the end in red
