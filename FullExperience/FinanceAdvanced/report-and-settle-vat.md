---
title: "Report and Settle VAT"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "VAT, settling"
  - "reporting VAT"
  - "settlement, reports"
  - "settlement, VAT"
  - "VAT, reporting"
ms.assetid: 88fd0739-f4ef-49e9-9a7d-04196686952a
caps.latest.revision: 5
ms.author: "sgroespe"
manager: "terryaus"
translation.priority.ht: 
  - "da-dk"
  - "de-at"
  - "de-ch"
  - "de-de"
  - "en-au"
  - "en-ca"
  - "en-gb"
  - "en-in"
  - "en-my"
  - "en-nz"
  - "en-ph"
  - "en-sg"
  - "en-zw"
  - "es-es"
  - "es-mx"
  - "fi-fi"
  - "fr-be"
  - "fr-ca"
  - "fr-ch"
  - "fr-fr"
  - "is-is"
  - "it-ch"
  - "it-it"
  - "nb-no"
  - "nl-be"
  - "nl-nl"
  - "ru-ru"
  - "sv-se"
---
# Report and Settle VAT
If you have set up the VAT features correctly, VAT is calculated and posted automatically.  
  
 You must report the volume of your trade with European Union \(EU\) countries\/regions to the tax authorities, even if no amount has to be settled. Refer to the guidelines provided by your country\/region's tax authorities for reporting requirements and instructions.  
  
 Every posting that involves VAT creates an entry in the **VAT Entries** window. These entries are used to calculate your VAT settlement amount \(payment or refund\) for a specific period.  
  
 You can also use general ledger entries to calculate the settlement amount if you set up accounts on the chart of accounts for this purpose. \(See the **Type** field on the VAT statement line.\) Note, this method does not follow the format used by the tax authorities on the VAT statement.  
  
 You can use a VAT statement to calculate the VAT settlement amount for a period. You can then print a VAT statement and copy the information onto a payment slip.  
  
 VAT is not calculated on sales to VAT\-liable companies in other EU countries\/regions. You must report the value of such sales separately. You can use the **VAT \- VIES Declaration Tax Auth.** report to produce the declaration.  
  
 You can use the **Calc. and Post VAT Settlement** batch job to close the VAT entries and transfer purchase and sales VAT amounts to the VAT settlement account.  
  
 The following table describes a sequence of tasks, with links to the topics that describe them. These tasks are listed in the order in which they are generally performed.  
  
|**To**|**See**|  
|------------|-------------|  
|Post a journal where the entire amount must be treated as VAT, for example, if you receive a VAT invoice from the tax authorities for imported goods.|[How to: Post Import VAT](../Finance/how-to-post-import-vat.md)|  
|Post a purchase invoice where the entire amount must be treated as VAT.|[How to: Post Import VAT with Purchase Invoices](../Finance/how-to-post-import-vat-with-purchase-invoices.md)|  
|View entries that have been created by posting VAT.|[How to: View VAT Entries](../Finance/how-to-view-vat-entries.md)|  
|Define how the VAT statement will be calculated.|[How to: Define VAT Statements](../Finance/how-to-define-vat-statements.md)|  
|Preview a VAT statement on screen before printing the statement.|[How to: Preview VAT Statements](../Finance/how-to-preview-vat-statements.md)|  
|Print a VAT statement that you can use to fill in the payment slip for the tax authorities.|[How to: Print VAT Statements](../Finance/how-to-print-vat-statements.md)|  
|Create a periodic VAT report that can be submitted to the tax authorities.|[VAT and VIES Report Setup](../Finance/vat-and-vies-report-setup.md)|  
|Print a VIES report for sales to other EU countries\/regions.|[VAT\- VIES Declaration Tax Auth\-duplicate](../Topic/\($%20R_19%20VAT-%20VIES%20Declaration%20Tax%20Auth%20$\)-duplicate.md)|  
|Close the open VAT entries and post the net settlement amount to the VAT settlement account.|[How to: Transfer VAT Amounts to the Settlement Account](../Finance/how-to-transfer-vat-amounts-to-the-settlement-account.md)|  
  
## See Also  
 [Type](assetId:///df666cfc-2511-4be7-8000-2cc231552477)   
 [Calc. and Post VAT Settlement](../Topic/\($%20B_20%20Calc.%20and%20Post%20VAT%20Settlement%20$\).md)   
 [Set Up VAT](../Finance/set-up-vat.md)   
 [How to: Record VAT](../Finance/how-to-record-vat.md)   
 [How to: Correct VAT](../Finance/how-to-correct-vat.md)   
 [Calc. and Post VAT Settlement](../Topic/\($%20B_20%20Calc.%20and%20Post%20VAT%20Settlement%20$\).md)