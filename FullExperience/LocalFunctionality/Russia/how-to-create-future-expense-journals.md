---
title: "How to: Create Future Expense Journals"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "future expenses, creating journals"
ms.assetid: 68d472ed-05ad-4a55-a3d9-55c51ff40983
caps.latest.revision: 2
ms.author: "edupont"
translation.priority.ht: 
  - "ru-ru"
---
# How to: Create Future Expense Journals
Future expense journals are used to post expenses to a special account on a monthly basis. These future expenses are later included as expenses. VAT is deducted when future expenses are included in current expenses.  
  
 You must select **Future Expenses** in the **\($ T\_80\_9 Type $\)** field of the **\($ N\_101 General Journal Templates $\)** window. In addition, be sure you select the **\($ T\_80\_12 Recurring $\)** and **\($ T\_80\_23 Copy VAT Setup to Jnl. Lines $\)** check boxes in the **\($ N\_101 General. Journal Templates $\)** window.  
  
### To create future expense journals  
  
1.  In the **Search** box, enter **VAT Posting Setup**, and then choose the related link. Use the **\($ N\_472 VAT Posting Setup $\)** window to create VAT posting groups. For more information, see [How to: Set Up VAT Product Posting Groups](../../Finance/how-to-set-up-vat-product-posting-groups.md) and [How to: Set Up VAT Business Posting Groups](../../Finance/how-to-set-up-vat-business-posting-groups.md).  
  
2.  On the **Settlement** FastTab, in the **\($ T\_325\_12408 VAT Settlement Template $\)** field, select a template.  
  
3.  Select a batch in the **\($ T\_325\_12409 VAT Settlement Batch $\)** field. This determines the batch where future expenses and VAT will be produced.  
  
4.  In the **Search** box, enter **Purchase Invoices**, and then choose the related link. Create a purchase invoice for the deferral general ledger account \(97\).  
  
5.  Create and post the payment and apply the invoice and payment.  
  
     VAT is not deducted at this time. It is deducted later, on a monthly basis through the Future Expense Journal.  
  
6.  In the **Search** box, enter **Future Expense Journals**, and then choose the related link.  
  
7.  In the **\($ N\_17333 Future Expense Journal $\)** window, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**\($ T\_5621\_7 FA Posting Date $\)**|Specifies the fixed asset posting date that is associated with the future expense journal.|  
    |**\($ T\_5621\_11 Document No. $\)**|Specifies the document number that is associated with the future expense journal.|  
    |**\($ T\_5621\_6 FA No. $\)**|Specifies the fixed asset number that is associated with the future expense journal.|  
    |**\($ T\_5621\_4 Depreciation Book Code $\)**|Specifies the depreciation book code that is associated with the future expense journal.|  
    |**\($ T\_5621\_5 FA Posting Type $\)**|Specifies the fixed asset posting type that is associated with the future expense journal. Fixed asset posting types include **Acquisition Cost**, **Depreciation**, **Write\-Down**, **Appreciation**, **Custom 1**, **Custom 2**, **Disposal**, **Maintenance**, **Salvage Value**, and **Transfer**.|  
    |**\($ T\_5621\_13 Description $\)**|Specifies the description that is associated with the future expense journal.|  
    |**\($ T\_5621\_12400 Location Code $\)**|Specifies the location code that is associated with the future expense journal.|  
    |**\($ T\_5621\_14 Amount $\)**|Specifies the amount that is associated with the future expense journal.|  
    |**\($ T\_5621\_17300 Depr. Amount w\/o Normalization $\)**|Specifies the depreciation amount without normalizations that is associated with the future expense journal.|  
    |**\($ T\_5621\_12450 Actual Quantity $\)**|Specifies the actual quantity that is associated with the future expense journal.|  
    |**\($ T\_5621\_12451 Calc. Quantity $\)**|Specifies the calculated quantity that is associated with the future expense journal.|  
    |**\($ T\_5621\_12452 Actual Amount $\)**|Specifies the actual amount that is associated with the future expense journal.|  
    |**\($ T\_5621\_12453 Calc. Amount $\)**|Specifies the calculated amount that is associated with the future expense journal.|  
    |**\($ T\_5621\_17302 Actual Remaining Amount $\)**|Specifies the actual remaining amount that is associated with the future expense journal.|  
    |**\($ T\_5621\_17 Salvage Amount $\)**|Specifies the salvage amount that is associated with the future expense journal.|  
    |**\($ T\_5621\_20 No. of Depreciation Days $\)**|Specifies the number of depreciation days that is associated with the future expense journal.|  
    |**\($ T\_5621\_21 Depr. Until FA Posting Date $\)**|Specifies if the depreciation until fixed asset posting date is used with the future expense journal.|  
    |**\($ T\_5621\_22 Depr. Acquisition Cost $\)**|Specifies if the depreciation acquisition cost is used with the future expense journal.|  
    |**\($ T\_5621\_33 Duplicate in Depreciation Book $\)**|Specifies the duplicate in depreciation book that is associated with the future expense journal.|  
    |**\($ T\_5621\_35 FA Error Entry No. $\)**|Specifies the fixed asset error entry number that is associated with the future expense journal.|  
  
8.  On the **Home** tab, in the **Process** group, choose **Post**. The amount entered in the **\($ T\_5621\_14 Amount $\)** field will be transferred from the Future Expenses account to the Current Expenses account. VAT will be calculated according to VAT setup \(percentage\) on the basis of the posted amount, and VAT deduction \(realized VAT\) will be posted.  
  
## See Also  
 [\($ N\_5607 Fixed Asset Setup $\)](../Topic/\($%20N_5607%20Fixed%20Asset%20Setup%20$\).md)   
 [Fixed Assets Accounting Setup](../../Finance/fixed-assets-accounting-setup.md)   
 [\($ N\_5600 Fixed Asset Card $\)](../Topic/\($%20N_5600%20Fixed%20Asset%20Card%20$\).md)   
 [How to: Set Up a Future Expense Card](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Russia/how-to-set-up-a-future-expense-card.md)