---
title: "How to: Customize FactBoxes"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "removing, fields"
  - "FactBoxes, ordering"
  - "removing, FactBoxes"
  - "adding, FactBoxes"
  - "FactBoxes, removing"
  - "FactBoxes, adding"
  - "restoring defaults"
  - "adding, fields"
  - "fields, removing"
  - "FactBoxes, customizing"
  - "fields, adding"
  - "customizing, FactBoxes"
  - "customizing, FactBox panes"
ms.assetid: 15ae2c44-a755-4cb8-b0e7-7fa543dfe88c
caps.latest.revision: 22
ms.author: "solsen"
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
  - "en-nz"
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
# How to: Customize FactBoxes
You can add or remove FactBoxes in the FactBox pane with the **Customize** dialog box. You use FactBoxes to see information that relates to the record that you have selected in the list or opened in a task page. You can select which FactBoxes to display in your FactBox pane. You can also customize FactBoxes to display only the fields that you need.  
  
> [!NOTE]  
>  Depending on the setting in the **UI Elements Removal** field in the [!INCLUDE[nav_admin](../BusinessFunctionality/LoggingAndTrackingEmailInteractions/includes/nav_admin_md.md)], only fields that you have permissions for will appear in the **Customize** window when you customize a FactBox. For more information, see [How to: Specify When UI Elements Are Removed](../Topic/How%20to:%20Specify%20When%20UI%20Elements%20Are%20Removed.md).  
  
 You can make multiple customizations of the same page based on different access points to the page. For example, you can customize that FactBoxes in the **Sales Orders** window look different when the window is opened from the **Customer Card** window than when it is opened from your Role Center. The point from which you access the page to be customized is recorded in that specific page customization. Accordingly, there may be multiple customization records for the same page under your logon, as you can see in the **Delete User Personalization** window.  
  
## Customizing the FactBox Pane  
  
#### To start customizing a FactBox Pane  
  
1.  On the **Application** menu ![Microsoft Dynamics NAV Application menu](../BusinessFunctionality/IntegratingWithMicrosoftDynamicsCRM/media/rtc_applicationmenu.png "RTC\_ApplicationMenu"), select **Customize**, and then choose **Customize This Page**.  
  
2.  In the **Customize \<Page Name\>** dialog box, select **FactBoxes**.  
  
#### To add FactBoxes  
  
1.  Select the FactBox that you want to add to the FactBox pane in the **Available FactBoxes** box.  
  
2.  Choose the **Add** button, and then choose the **OK** button.  
  
#### To remove FactBoxes  
  
1.  Select the FactBoxes in the **Show FactBoxes in this order** box.  
  
2.  Choose the **Remove** button, and then choose the **OK** button.  
  
#### To change the order of the FactBoxes  
  
-   Select the FactBox that you want to move in the **Show FactBoxes in this order** box, and then choose the **Move Up** or **Move Down** buttons until it is positioned where you want it.  
  
#### To restore default settings  
  
-   Choose the **Restore Defaults** button, and then choose the **OK** button.  
  
    > [!NOTE]  
    >  All the FastBox Pane customization that you have ever made for this page under your current user logon or since you last used the **Restore Defaults** button are canceled. The FactBox Pane is reset to the default configuration for your profile. For more information, see [How to: Cancel UI Personalization](../SetupAndAdministration/how-to-cancel-ui-personalization.md).  
  
## Customizing FactBoxes  
  
#### To start customizing a FactBox  
  
1.  Pause on the FactBox with the pointer until the **Actions**![Action Menu icon](../DesignAndEngineering/media/actionmenuicon.png "actionMenuIcon") menu is displayed.  
  
2.  Choose **Actions**, and then choose **Customize**.  
  
#### To add fields to FactBoxes  
  
-   Select the field that you want to add in the **Available fields** box, choose the **Add** button, and then choose the **OK** button.  
  
#### To remove fields from FactBoxes  
  
-   Select the field that you want to remove in the **Fields shown** box, and then choose the **Remove** button.  
  
#### To restore default settings  
  
-   In the **Customize** window, choose the **Restore Defaults** button, and then choose the **OK** button.  
  
    > [!NOTE]  
    >  All customization of FactBoxes that you have ever made for this page under your current user logon or since you last used the **Restore Defaults** button are canceled. The FactBoxes on the page are reset to the default configuration for your profile. For more information, see [How to: Cancel UI Personalization](../SetupAndAdministration/how-to-cancel-ui-personalization.md).  
  
## See Also  
 [Personalize the User Interface](../SetupAndAdministration/-$-s_personalization-personalize-the-user-interface-$-.md)   
 [How to: Customize Ribbons](../SetupAndAdministration/how-to-customize-ribbons.md)   
 [How to: Customize FastTabs](../SetupAndAdministration/how-to-customize-fasttabs.md)   
 [How to: Specify When UI Elements Are Removed](../Topic/How%20to:%20Specify%20When%20UI%20Elements%20Are%20Removed.md)   
 [How to: Cancel UI Personalization](../SetupAndAdministration/how-to-cancel-ui-personalization.md)   
 [Delete User Personalization](../Topic/\($%20N_9191%20Delete%20User%20Personalization%20$\).md)   
 [Customize the User Interface](../SetupAndAdministration/customize-the-user-interface.md)   
 [Working with Product Name](../WorkingWithDynamics/working-with-$-p_1-product-name-$-.md)   
 [Learn About the RoleTailored Design](../GettingStarted/learn-about-the-roletailored-design.md)