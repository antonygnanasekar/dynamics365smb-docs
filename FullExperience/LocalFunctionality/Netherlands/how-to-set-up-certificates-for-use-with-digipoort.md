---
title: "How to: Process Response Messages from Tax Authorities"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "response messages"
ms.assetid: 8769f5d3-6414-4355-adc3-d5e4fd5bebea
caps.latest.revision: 19
ms.author: "edupont"
manager: "terryaus"
translation.priority.ht: 
  - "nl-nl"
---
# How to: Process Response Messages from Tax Authorities
When you submit a VAT or ICP declaration to the tax authorities electronically, they will process the declaration and send you a message in response.  
  
 You can import the response into [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] by using the **\($ B\_11408 Receive Response Messages $\)** batch job. The response message will contain the status of the declaration.  
  
### To import messages from the tax authorities' server  
  
1.  In the **Search** box, enter **\($ N\_11416 Elec. Tax Decl. Response Msgs. $\)**, and then choose the related link.  
  
2.  On the **Home** tab, in the **Process** group, choose **\($ B\_11408 Receive Response Messages $\)**.  
  
3.  On the **Options** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**CA Certificate Encryption Password**|The password that was used to encrypt the Certificate Authorities' certificates.|  
    |**User Certificate Password**|The password that is used to encrypt the user certificates.|  
  
4.  Choose the **OK** button.  
  
### To process the response messages from the tax authorities  
  
1.  In the **Search** box, enter **\($ N\_11416 Elec. Tax Decl. Response Msgs. $\)**, and then choose the related link.  
  
2.  On the **Home** tab, in the **Process** group, choose **\($ B\_11406 Process Response Messages $\)**.  
  
3.  In the **\($ B\_11406 Process Response Messages Batch Job $\)** window, on the **Elec. Tax Decl. Response Msg**. FastTab, select the appropriate filters.  
  
4.  Choose the **OK** button.  
  
     The processed information about the response message is displayed in the **\($ N\_11416 Elec. Tax Decl. Response Msgs. $\)**. window.  
  
5.  To export a message or attachment, on the **Actions** tab, in the **Functions** group, choose **Export Response Message** or **Export Response Attachment**.  
  
## See Also  
 [Electronic VAT and ICP Declarations](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/electronic-vat-and-icp-declarations.md)   
 [How to: Set Up VAT Categories](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/how-to-set-up-vat-categories.md)   
 [How to: Create Electronic VAT and ICP Declarations](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/how-to-create-electronic-vat-and-icp-declarations.md)   
 [\($ T\_11409 Elec. Tax Declaration Header Table $\)](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/-$-t_11409-elec.-tax-declaration-header-table-$-.md)   
 [\($ T\_11413 Elec. Tax Decl. Response Msg. Table $\)](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/-$-t_11413-elec.-tax-decl.-response-msg.-table-$-.md)   
 [\($ B\_11408 Receive Response Messages Batch Job $\)](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/-$-b_11408-receive-response-messages-batch-job-$-.md)   
 [\($ B\_11406 Process Response Messages Batch Job $\)](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Netherlands/-$-b_11406-process-response-messages-batch-job-$-.md)