---
title: "How to: Calculate Accelerated Depreciation"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "calculating, accelerated depreciation"
  - "accelerated depreciation, calculating"
ms.assetid: 95c9315b-ec89-491f-920d-5760a0798277
caps.latest.revision: 34
ms.author: "edupont"
manager: "terryaus"
translation.priority.ht: 
  - "fr-fr"
---
# How to: Calculate Accelerated Depreciation
In [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)], you calculate periodic depreciation for fixed assets by using the **Calculate Depreciation** batch job. The fixed asset depreciation book that is linked to the fixed asset defines the depreciation method, the starting date for depreciation, and the fixed asset posting group that is used in the batch job.  
  
 If a fixed asset depreciation book is integrated with the general ledger, then it is called an *accounting depreciation book*. If a fixed asset depreciation book is not integrated with the general ledger, then it is called a *tax depreciation book*.  
  
 You can only calculate the accelerated depreciation for fixed assets that have an accounting depreciation book and a tax depreciation book. For more information about setting up tax depreciation books and accounting depreciation books for fixed assets, see [How to: Set Up Accelerated Depreciation](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-set-up-accelerated-depreciation.md).  
  
 Entries are transferred to the fixed asset general journal when you select an accounting depreciation book in the batch job. Entries are transferred to the fixed asset journal when you select the tax depreciation book.  
  
### To calculate accelerated depreciation  
  
1.  In the **Search** box, enter **Calculate Depreciation**, and then choose the relevant link.  
  
2.  In the **Calculate Depreciation** window, on the **Options** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Depreciation Book**|The unique identification code for the accounting depreciation book.|  
    |**FA Posting Date**|Specify the ending date for the depreciation calculation, if this is the first depreciation entry for the asset. The depreciation starting date that is defined in the **FA Depreciation Books** window is used as the starting date for the depreciation calculation. If you have already depreciated the asset, the fixed asset posting date of the last depreciation entry is used as the starting date for the depreciation calculation.|  
    |**Use Force No. of Days**|Select to use the number of days in the **Force No. of Days** field for the depreciation calculation.|  
    |**Force No. of Days**|The number of days for the depreciation calculation. You can only enter a number in this field if the **Use Force No of Days** check box is selected.|  
    |**Posting Date**|The posting date for the calculated depreciation.<br /><br /> You can leave this field blank if the **Use Same FA \+ G\/L Posting Dates** field in the accounting depreciation book is selected. The posting date is copied to the resulting journal lines. For more information, see [Use Same FA\+G\-L Posting Dates](../Topic/\($%20T_5611_19%20Use%20Same%20FA+G-L%20Posting%20Dates%20$\).md).|  
    |**Document No.**|The document number for the fixed asset journal batch. Leave this field blank if you have set up a numbering series for the fixed asset journal batch in the **No. Series** window. For more information, see [No. Series](assetId:///18dc626f-cdf2-4bd9-b1ab-d98927ce4c3b).|  
    |**Posting Description**|The posting description for the fixed asset journal entries.|  
    |**Insert Bal. Account**|Select to automatically insert balancing accounts in the resulting journal. The **Calculate Depreciation** batch job only uses balancing accounts that are defined in the [FA Posting Group](../Topic/\($%20T_5606%20FA%20Posting%20Group%20$\).md).|  
  
3.  On the **Fixed Asset** FastTab, select the appropriate filters.  
  
4.  Choose the **OK** button.  
  
     The accelerated depreciation for the fixed asset is calculated.  
  
## See Also  
 [Accelerated Depreciation](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/accelerated-depreciation.md)   
 [How to: Set Up Accelerated Depreciation](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-set-up-accelerated-depreciation.md)   
 [Fixed Asset](../Topic/\($%20T_5600%20Fixed%20Asset%20$\).md)   
 [Fixed Asset Card](../Topic/\($%20N_5600%20Fixed%20Asset%20Card%20$\).md)   
 [Set Up Depreciation](../../Finance/set-up-depreciation.md)   
 [Use Same FA\+G\-L Posting Dates](../Topic/\($%20T_5611_19%20Use%20Same%20FA+G-L%20Posting%20Dates%20$\).md)   
 [FA Posting Group](../Topic/\($%20T_5606%20FA%20Posting%20Group%20$\).md)   
 [No. Series](assetId:///18dc626f-cdf2-4bd9-b1ab-d98927ce4c3b)   
 [Depreciation Book](../Topic/\($%20T_5611%20Depreciation%20Book%20$\).md)   
 [FA Depreciation Books](../Topic/\($%20N_5619%20FA%20Depreciation%20Books%20$\).md)   
 [Calculate Depreciation](../Topic/\($%20B_5692%20Calculate%20Depreciation%20$\).md)