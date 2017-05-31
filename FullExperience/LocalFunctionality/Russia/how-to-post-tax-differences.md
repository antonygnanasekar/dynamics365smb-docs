---
title: "How to: Post Tax Differences"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "posting, tax differences"
  - "tax differences, posting"
  - "taxes"
ms.assetid: 27ee539e-c1e3-40cd-b2fd-86e737eefb0d
caps.latest.revision: 2
ms.author: "edupont"
translation.priority.ht: 
  - "ru-ru"
---
# How to: Post Tax Differences
The **\($ N\_17306 Tax Difference Journal $\)** is used to create and post tax difference transactions. Tax differences are variations in tax amounts caused by the different rules for recognizing income and expenses between entries for book accounting and tax accounting.  
  
 You can use the **\($ N\_17306 Tax Difference Journal $\)** to manually create tax difference journal entries or you can modify existing entries created by periodic tax difference calculation activities. When you post the **\($ N\_17306 Tax Difference Journal $\)**, tax differences entries are posted to the selected posting groups.  
  
### To post tax differences  
  
1.  In the **Search** box, enter **Tax Difference Journal**, and then choose the related link.  
  
2.  Fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**\($ T\_17305\_4 Posting Date $\)**|Enter the transaction date.|  
    |**\($ T\_17305\_5 Document No. $\)**|Enter the document number from the source transaction.|  
    |**\($ T\_17305\_23 Description $\)**|Enter a description for the transaction.|  
    |**\($ T\_17305\_6 Tax Diff. Type $\)**|Select if the tax difference is **Constant** or **Temporary**.|  
    |**\($ T\_17305\_7 Tax Diff. Code $\)**|Select an identifying income or expense code that defines the source of the tax difference.|  
    |**\($ T\_17305\_32 Source Type $\)**|Select the source of tax difference. The options include **Future Expense**, **Fixed Asset**, and **Intangible Asset**.|  
    |**\($ T\_17305\_33 Source No. $\)**|If the **\($ T\_17305\_32 Source Type $\)** is **Future Expense**, enter an identifying code for the future period expenses.  Otherwise, leave this field blank.|  
    |**\($ T\_17305\_9 Jurisdiction Code $\)**|Select the identifying code for the jurisdiction that is used to calculate taxable profits and losses for tax differences.|  
    |**\($ T\_17305\_10 Norm Code $\)**|Select the identifying code for the norm jurisdiction that is used to calculate taxable profits and losses for the tax differences.|  
    |**\($ T\_17305\_11 Tax Factor $\)**|Enter the profit tax rate that is used to calculate tax differences.|  
    |**\($ T\_17305\_13 Amount \(Base\) $\)**|Enter an expense amount based on book accounting transactions. This information is used if the tax difference calculation is for a set period of time.|  
    |**\($ T\_17305\_14 Amount \(Tax\) $\)**|Enter an expense amount based on tax accounting transactions. This information is used if the tax difference calculation is for a set period of time.|  
    |**\($ T\_17305\_15 Difference $\)**|Enter the value of the difference between the book accounting and tax accounting transactions.|  
    |**\($ T\_17305\_29 YTD Amount \(Base\) $\)**|Enter the year\-to\-date value of the expense or income amount based on the book accounting data.|  
    |**\($ T\_17305\_30 YTD Amount \(Tax\) $\)**|Enter the year\-to\-date value of the expense or income amount based on the tax accounting data.|  
    |**\($ T\_17305\_31 YTD Difference $\)**|Enter the year\-to\-date value of the difference between the book accounting and tax accounting transactions.|  
    |**\($ T\_17305\_37 Tax Diff. Calc. Mode $\)**|Specifies the difference of the counting mode. If **Balance** is selected, the difference will be calculated by a creating total starting from the start of the year. If not selected, the difference will be created for the current period.|  
    |**\($ T\_17305\_16 Tax Amount $\)**|Specifies the counting result. The value of this field will correct the profit tax in the book accounting transactions.|  
    |**\($ T\_17305\_17 Asset Tax Amount $\)**|Specifies the calculated asset tax amount.|  
    |**\($ T\_17305\_18 Liability Tax Amount $\)**|Specifies the calculated liability tax amount.|  
    |**\($ T\_17305\_19 Disposal Tax Amount $\)**|Specifies the tax amount that is written off at disposal of an item.|  
    |**\($ T\_17305\_20 DTA Starting Balance $\)**|Specifies the starting disposal tax amount before counting.|  
    |**\($ T\_17305\_21 DTL Starting Balance $\)**|Specifies the starting disposal tax liability amount before counting.|  
    |**\($ T\_17305\_27 DTA Ending Balance $\)**|Specifies the disposal tax amount after counting.|  
    |**\($ T\_17305\_28 DTL Ending Balance $\)**|Specifies the disposal tax liability amount after counting.|  
    |**\($ T\_17305\_26 Disposal Mode $\)**|Select if you want to write down the tax difference or transform it into a constant difference.|  
    |**\($ T\_17305\_22 Disposal Date $\)**|Enter the date of the item’s disposal.|  
    |**\($ T\_17305\_36 Partial Disposal $\)**|Select if you want to dispose of an item that causes differences in the expense or income code. If this field is not selected, the tax differences are written off.|  
  
3.  On the **Action Pane**, in the **Process** actions group, choose the **Post** button. The tax difference journal transaction is posted.  
  
4.  On the **Action Pane**, in the **Process** actions group, choose **Ledger Entries** to open the **\($ N\_17307 Tax Diff. Ledger Entry $\)** window and review the posted entries.  
  
## See Also  
 [Tax Differences](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Russia/tax-differences.md)   
 [Setting up Tax Difference Calculation](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Russia/setting-up-tax-difference-calculation.md)   
 [Tax Accounting](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Russia/tax-accounting.md)   
 [Tax Reports](assetId:///e42ca8e7-1cee-4fb8-9f71-e596f29cabc3)   
 [Tax Registers](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Russia/tax-registers.md)   
 [How to: Create Tax Registers](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Russia/how-to-create-tax-registers.md)