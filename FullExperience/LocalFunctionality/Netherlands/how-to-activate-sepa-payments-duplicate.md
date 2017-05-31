---
title: "How to: Activate SEPA Payments-duplicate"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "vendor payments, SEPA"
  - "SEPA, setting up"
ms.assetid: 882865ab-7541-4cdb-aeb4-cfdbb512571a
caps.latest.revision: 20
ms.author: "edupont"
manager: "terryaus"
translation.priority.ht: 
  - "nl-nl"
---
# How to: Activate SEPA Payments-duplicate
To submit vendor payments electronically in Single Euro Payments Area \(SEPA\) ISO 20022 payment format, you must set up prerequisites for enabling SEPA payments.  
  
 In the following procedures, the first four describe how to enable SEPA payments, and the remaining two relate to the individual vendors.  
  
### To enable countries\/regions for SEPA  
  
1.  In the **Search** box, enter **\($ N\_10 Countries\/Regions $\)**, and then choose the related link.  
  
2.  On the **Home** tab, in the **Manage** group, choose **Edit List**.  
  
3.  Select the **\($ T\_9\_11400 SEPA Allowed $\)** check box for each country or region that you want to enable for SEPA.  
  
4.  Choose the **OK** button.  
  
### To enable bank accounts for SEPA  
  
1.  In the **Search** box, enter **Bank Accounts**, and then choose the related link.  
  
2.  Select the bank account that you want to enable for SEPA, and then, on the **Home** tab, in the **Manage** group, choose **Edit**.  
  
3.  On the **General** FastTab, in the **\($ T\_270\_35 Country\/Region Code $\)** field, select the appropriate code.  
  
    > [!NOTE]  
    >  The specified country\/region code must be enabled for SEPA as described in the previous procedure.  
  
4.  Enter a value in the **\($ T\_270\_20 Min. Balance $\)** field.  
  
5.  On the **Transfer** FastTab, in the **\($ T\_270\_111 SWIFT Code $\)** field, enter a code.  
  
6.  Choose the **OK** button.  
  
### To set up a SEPA ISO 20022 export protocol  
  
1.  In the **Search** box, enter **\($ N\_11000012 Export Protocols $\)**, and then choose the related link.  
  
2.  In the **\($ N\_11000012 Export Protocols $\)** window, on the **Home** tab, choose **New**.  
  
3.  Fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**\($ T\_11000005\_1 Code $\)**|Sets the export protocol code, such as **SEPA ISO20022**.|  
    |**\($ T\_11000005\_2 Description $\)**|Provides the description for the export protocol.|  
    |**\($ T\_11000005\_10 Check ID $\)**|Sets the ID for the codeunit to check payment, such as **11000010**.|  
    |**\($ T\_11000005\_30 Check Name $\)**|Sets the name of the codeunit.|  
    |**\($ T\_11000005\_8 Export Protocol Type $\)**|Specifies the type of the export protocol:<br /><br /> -   **Report**<br />-   **XMLPort**|  
    |**\($ T\_11000005\_11 Export ID $\)**|Sets the ID for the batch job to export payment, such as **11000011**.<br /><br /> If you select XMLPort as your export protocol type, then choose an ID such as **1000**.|  
    |**\($ T\_11000005\_31 Export Name $\)**|The name of the batch job.|  
    |**\($ T\_11000005\_12 Docket ID $\)**|Sets the ID for the batch job to inform the contact on combined payments, such as **11000004**.<br /><br /> This does not apply to XMLPort protocol types.|  
    |**\($ T\_11000005\_32 Docket Name $\)**|The name of the docket report.|  
    |**\($ T\_11000005\_21 Default File Names $\)**|Sets the location to export payment and collection data.|  
  
4.  Choose the **OK** button.  
  
### To enable transaction modes for SEPA  
  
1.  In the **Search** box, enter **Transaction Modes**, and then choose the related link.  
  
2.  Select the transaction mode that you want to enable for SEPA, and then, on the **Home** tab, in the **Manage** group, choose **Edit**.  
  
3.  In the **\($ N\_11000011 Transaction Mode Card $\)** window, on the **Paym. Proposal** FastTab, in the **\($ T\_11000004\_12 Export Protocol $\)** field, select the SEPA export protocol that you have created, such as **SEPA ISO20022**.  
  
4.  Choose the **OK** button.  
  
### To verify vendor payment transaction modes for SEPA  
  
1.  In the **Search** box, enter **Vendors**, and then choose the related link.  
  
2.  Select the vendor that you want to verify the transaction mode for, and then, on the **Home** tab, in the **Manage** group, choose **View**.  
  
3.  On the **Payments** FastTab, in the **\($ T\_23\_11000000 Transaction Mode Code $\)** field, verify that the vendor payment transaction mode is one that has been enabled for SEPA.  
  
4.  Choose the **OK** button.  
  
### To set up vendor bank accounts for SEPA  
  
1.  In the **Search** box, enter **Vendors**, and then choose the related link.  
  
2.  Select the relevant vendor, and then, on the **Navigate** tab, in the **Vendor** group, choose **Bank Accounts**.  
  
3.  Select the vendor bank account to set up for SEPA, and then, on the **Home** tab, in the **Manage** group, choose **Edit**.  
  
4.  On the **Transfer** FastTab, in the **\($ T\_288\_24 IBAN $\)** and **\($ T\_288\_25 SWIFT Code $\)** fields, enter the international bank identifier code of the bank where the vendor has the account.  
  
5.  Choose the **OK** button.  
  
## See Also  
 [Single EURO Payments Area \(SEPA\)](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/single-euro-payments-area-sepa-.md)   
 [How to: Submit Vendor Payments Electronically in SEPA ISO 20022 Payment Format](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/how-to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format.md)   
 [\($ N\_11000012 Export Protocols Window $\)](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/-$-n_11000012-export-protocols-window-$-.md)