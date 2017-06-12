---
title: "Italian VAT"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "VAT reporting, about"
  - "service tariffs"
  - "VAT, in Italy"
ms.assetid: 0cad8837-bc4a-4ad7-bf39-4f8c1bd09709
caps.latest.revision: 33
ms.author: "edupont"
manager: "terryaus"
translation.priority.ht: 
  - "it-it"
---
# Italian VAT
Companies must pay VAT to the state for most purchased goods and services. VAT can be deducted if the goods or services purchased by a company are used in the production of its income.  
  
 In [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)], you can define periodic VAT reports in the **VAT Report** window. You can fill in the lines based on VAT entries, and then export the VAT report to the appropriate authorities.  
  
## VAT Codes and Rates  
 VAT codes and rates must be set up even though some transactions are not subject to VAT rates. There are also many VAT\-liable operations that are subject to a zero VAT rate by provision of the law.  
  
 The related VAT code is printed for each invoice line. Invoices for VAT transaction entries that are not subject to VAT rates must be recorded and printed with a note stating that VAT is not owed.  
  
### Computing VAT  
 VAT is computed for transactions to comply with the rules in effect on that the day the transactions occur. Thus, the date on which a transaction legally occurs must be tracked when recording transactions.  
  
### Dates  
 The date of issue is the document date and the date of registration is the posting date. Reporting date filters are based on the posting dates. This is changed from the previous behavior in which reporting date filters were based on the Operation Occured Date.  
  
### Non\-deductible VAT  
 VAT cannot be deducted for some purchases because of:  
  
-   The type of goods or services purchased – VAT is fully or partially non\-deductible by provision of the law on goods like cars, mobile phones, food purchased at restaurants, and so on.  
  
-   Partially deductible pro\-rated VAT – VAT is pro\-rated according to the ratio between sales operations for which VAT is owed, and all operations performed. VAT exceeding this ratio cannot be deducted.  
  
## Service Tariffs  
 The European Union \(EU\) has issued directives that change the VAT reporting for cross\-border trade of goods and services in the EU.  
  
 In Italy, the EU sales list \(Intrastat\) and annual listing reports are updated to include services. This involves a change in the reporting format. A new table for service tariffs is added so that companies can classify services that must be included in the Intrastat report. Users must add the relevant service tariff to all documents that are for cross\-border transactions. The service tariff specified on the **Foreign Trade** FastTab for the document can be modified in each line in the document.  
  
## VAT Transaction Reports  
 You must submit periodic reports to the tax authorities, which list transactions that include VAT with amounts over a specified threshold. The VAT transaction reports are created based on transactions with customers or vendors from a country\/region that is outside the EU and is not blacklisted. Transactions with customers or vendors from EU countries\/regions are reported through **Intrastat** reports. Transactions with customers or vendors from countries\/regions that are blacklisted are reported through the **Blacklist Communication Report** report. [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] provides support for the following transaction types:  
  
|||  
|-|-|  
|**Transaction Type**|**Supported**|  
|FE \- Customer invoices \(factures issued\)|Yes|  
|FR \- Vendor invoices \(factures received\)|Yes|  
|NE \- Customer credit notes \(notes issued\)|Yes|  
|NR \- Vendor credit notes \(notes received\)|Yes|  
|DF \- Transactions without invoices \(direct invoices\) \(customer\)|No|  
|FN \- Customers invoices, when customer is non\-resident|Yes|  
|SE \- Vendor invoices, when vendor is non\-resident|Yes **Note:**  The purchase of services is assumed, but differentiation between service and goods is left for the user to implement.|  
  
 [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] does not report the following types of transactions:  
  
-   Prepayment invoices, because the total amount will be reported at the time of the final invoice.  
  
-   Operations without an invoice, for example, VAT entries posted via general ledger accounts, because a VAT registration number, a fiscal code, or a customer or vendor reference is required for inclusion in a report.  
  
-   Self\-billed transactions, which are not supported.  
  
 The VAT transactions reports include lines where the amount is over the threshold and lines that must be included for other legal reasons. The threshold amount is set by the Italian authorities.  
  
 Document lines contain a field to indicate if the line must be included in the VAT transaction reports. The **Include in VAT Transac. Rep.** fields are selected automatically based on the day of the transaction and a comparison with the threshold amount for the calendar year. If sales lines are related to a blanket order, the threshold is compared to the amount for the blanket order. This only applies to sales line of type **Item**. For service lines, the comparison is made with the service contract amount.  
  
> [!NOTE]  
>  Credit memos are included in the VAT transaction report if the customer or vendor is from a country\/region that is outside the EU and is not blacklisted.  
  
 When you post credit memos, you must update the **Refers to Period** field to specify the relevant period. The VAT transaction reports will include credit memos where the **Refers to Period** field is set to **Current Calendar Year** or **Previous Calendar Year**.  
  
 [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] adds credit memos to the VAT reports in different ways depending on the application status and the value of the **Refers to Period** field. The following table describes the scenarios.  
  
|Scenario|Impact|  
|--------------|------------|  
|A credit memo is applied to a single invoice.<br /><br /> The **Refers to Period** field is set to **Current Calendar Year**.|The **Invoice No.** field will be set to the document number of the invoice.<br /><br /> The **Invoice Date** field will be set to the date that is specified in the **Operation Occurred Date** field<br /><br /> [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] will deduct the credit memo amount from the amount of the original invoice. If the resulting amount is above the threshold, both the invoice and credit memo will be included in the VAT transactions report. If the resulting amount is below the threshold, neither invoice or credit memo will be included in the VAT transactions report.|  
|A credit memo is applied to multiple invoices, or it is not applied.<br /><br /> The **Refers to Period** field is set to **Current Calendar Year**.|The **Invoice Date** field will be set to the last day of the year that is specified in the **Operation Occurred Date** field. For example, if the **Operation Occurred Date** field is **07\-11\-11**, the **Invoice Date** field will be set to **31\-12\-11**.<br /><br /> Only the credit memo will be included in the VAT transactions report.|  
|A credit memo is applied to multiple invoices, or it is not applied.<br /><br /> The **Refers to Period** field is set to **Previous Calendar Year**.|The **Invoice Date** field will be set to the last day of the year before the date that is specified in the **Operation Occurred Date** field. For example, if the **Operation Occurred Date** field is **07\-11\-11**, the **Invoice Date** field will be set to **31\-12\-10**.<br /><br /> Only the credit memo will be included in the VAT transactions report.|  
  
 When service contracts are compared with the threshold, the **Annual Amount** field is converted to your local currency \(LCY\). The conversion is based on the **Currency Code** field and the exchange rate on the date in the **Starting Date** field for the service contract.  
  
 Transactions with reverse charges are not included in the VAT transaction reports. Transactions with prepayments are also not included in the VAT transaction reports.  
  
 To prepare your data for these reports, you must set up VAT posting to include VAT transaction report amounts. When a transaction such as posting a sales invoice is made that uses this VAT posting setup, [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] checks if the transaction meets the threshold amounts. The check is based on document lines because a document can contain lines that must be included in the VAT transaction report and lines that must be excluded. The VAT transaction reports must only contain the lines that must be submitted, so [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] compares amounts against the threshold for each line instead of for a document. For more information, see [How to: Prepare for VAT Transactions Reports](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/how-to-prepare-for-vat-transactions-reports.md).  
  
 You must submit a VAT transactions report electronically to the tax authorities. For more information, see [How to: Create Electronic VAT Transactions Reports](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/how-to-create-electronic-vat-transactions-reports.md).  
  
## See Also  
 [How to: Create a VAT Combination Setup](../../Finance/how-to-create-a-vat-combination-setup.md)   
 [How to: Prepare for VAT Transactions Reports](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/how-to-prepare-for-vat-transactions-reports.md)   
 [How to: Create Electronic VAT Transactions Reports](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/how-to-create-electronic-vat-transactions-reports.md)   
 [How to: Submit VAT Statements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/how-to-submit-vat-statements.md)   
 [How to: Update VAT Transactions Data](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/how-to-update-vat-transactions-data.md)   
 [How to: Report Trade with Customers and Vendors in Blacklist Countries\-Regions](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/how-to-report-trade-with-customers-and-vendors-in-blacklist-countries-regions.md)   
 [Annual VAT Comm. \- 2010](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/-$-r_12126-annual-vat-comm.-2010-$-.md)   
 [Italy Local Functionality](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/italy-local-functionality.md)