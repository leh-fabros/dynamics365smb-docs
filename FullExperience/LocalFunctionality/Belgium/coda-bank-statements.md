---
title: "CODA Bank Statements"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "bank statements, CODA"
  - "CODA, bank statements"
ms.assetid: ad26695d-6f55-4a48-9ed8-dd9e517e5f78
caps.latest.revision: 2
ms.author: "edupont"
translation.priority.ht: 
  - "fr-be"
  - "nl-be"
---
# CODA Bank Statements
The Coded Statement of Account \(CODA\) is a national banking standard, designed by the Belgian Banker's Association, which allows you to automatically process electronic bank statements.  
  
 Each type of transaction in a CODA statement is assigned a unique code. [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] uses this code to interpret transactions and apply them to the corresponding ledger entries.  
  
## Applying Statement Lines  
 When you have imported a CODA statement, you can apply the statement lines to existing ledger entries, based on the information in the **Transaction Coding** table.  
  
 If the transaction coding of the statement line is not found, [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] will stop processing and continue with the next statement line. If you select the **Default Posting** field, the statement line will be used as a default posting.  
  
 If the transaction coding of the statement line is found, the statement lines will be matched to the following account types and corresponding account numbers:  
  
-   General ledger \- If the account type is general ledger account, the statement line is posted on the corresponding general ledger account.  
  
-   Customer or vendor \- If the account type is customer or vendor, a matching customer or vendor ledger entry is found based on the following criteria:  
  
    -   If a ledger entry is found using the standard format, the ledger entry will be matched to the statement line and the application status will be set to **Applied**. If the ledger entry does not use the standard format, the bank account number of the customer or vendor is used to find the customer or vendor.  
  
    -   If no ledger entry with a matching remaining amount is found, the customer or vendor account is used and the application status will be set to **Partly Applied**.  
  
    -   If the bank account number is used to find the customer or vendor, a matching ledger entry is found based on the amount of the statement line. If the amount is found, the statement line is matched to the corresponding ledger entry and the application status will be set to **Applied**.  
  
    -   If the bank account number cannot be used to find the customer or vendor, [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] will either stop processing the current line or use the line as a default posting, before continuing with the next statement line.  
  
 You can run the process as many times as you like. Only statement lines with a blank application status will be applied.  
  
 When you have applied all statement lines to a general ledger account or to a matching customer ledger entry or vendor ledger entry, you are ready to post the CODA statement lines. For more information, see [How to: Automatically Transfer and Post CODA Statements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-automatically-transfer-and-post-coda-statements.md) or [How to: Manually Transfer and Post CODA Statements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-manually-transfer-and-post-coda-statements.md).  
  
## See Also  
 [Belgian Electronic Banking](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/belgian-electronic-banking.md)   
 [How to: Set Up Bank Accounts for CODA](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-set-up-bank-accounts-for-coda.md)   
 [How to: Set Up IBLC\-BLWI Transaction Codes](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-set-up-iblc-blwi-transaction-codes.md)   
 [How to: Import CODA Statements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-import-coda-statements.md)   
 [How to: Apply CODA Statements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-apply-coda-statements.md)   
 [How to: Create Financial Journals](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-create-financial-journals.md)   
 [How to: Automatically Transfer and Post CODA Statements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-automatically-transfer-and-post-coda-statements.md)   
 [How to: Manually Transfer and Post CODA Statements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Belgium/how-to-manually-transfer-and-post-coda-statements.md)