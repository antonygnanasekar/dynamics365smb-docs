---
title: "How to: Create Assembly BOMs"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "assembly, BOM"
  - "assembly BOMs, creating"
  - "materials, structure"
ms.assetid: 86521a84-e208-4693-8411-d175ade70d3b
caps.latest.revision: 14
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
# How to: Create Assembly BOMs
Assembly BOMs specify which components or resources are required to assemble the item that the assembly BOM represents. Assembly BOMs usually contain items but can also contain one or more resources that perform the assembly work. For more information, see [\($ T\_90\_20 Resource Usage Type $\)](../Topic/\($%20T_90_20%20Resource%20Usage%20Type%20$\).md).  
  
 Assembly BOMs can be multilevel, which means that a component on the assembly BOM can be an assembly item itself. This is specified with the **Yes** value in the **Assembly BOM** field on the assembly BOM line. Multilevel assembly BOMs can have special requirements in certain cases, such as availability, planning, and standard cost calculation. For more information about how multilevel manufacturing or assembly items are handled in planning, see [How to: Run MPS and MRP](../OperationsPlanning/how-to-run-mps-and-mrp.md). For more information about how to calculate an assembly item’s cost at all levels, see [How to: Calculate the Standard Cost of Assembly BOMs](../Finance/how-to-calculate-the-standard-cost-of-assembly-boms.md).  
  
 When you enter the assembly item on an assembly order header, the assembly BOM components are automatically filled into the assembly order lines and are then ready to be consumed in the assembly process. For more information, see [How to: Assemble Items](../WarehouseActivities/how-to-assemble-items.md).  
  
 There are two steps to creating an assembly BOM:  
  
-   Setting up a new item card.  
  
-   Defining the BOM structure.  
  
### To create an assembly BOM  
  
1.  In the **Search** box, enter **Items**, and then choose the related link.  
  
2.  Create a new item. On the **Home** tab, in the **New** group, choose **New**. Fill in the required fields on the item card. For more information, see [How to: Register New Products](../DesignAndEngineering/how-to-register-new-products.md).  
  
3.  On the **Navigate** tab, in the **Assembly\/Production** group, choose the **Assembly** button, and then choose **Assembly BOM**.  
  
4.  To enter components in the assembly BOM, in the **Type** field, enter **Item**. In the **No.** field, select an item.  
  
    > [!NOTE]  
    >  If the component that you enter is an assembly item, then the **Assembly BOM** field contains **Yes**.  
  
5.  To enter a resource in the assembly BOM, in the **Type** field, enter **Resource**. In  the **No.** field, select a resource.  
  
6.  Leave the **Type** field blank if you want to enter a text on the assembly line, such as to describe an item or an assembly step.  
  
7.  In the **Quantity per** field, define how many units of the item or resource go into the assembly BOM.  
  
8.  Choose the **OK** button.  
  
## See Also  
 [\($ N\_36 Assembly BOM $\)](../Topic/\($%20N_36%20Assembly%20BOM%20$\).md)   
 [\($ N\_900 Assembly Order $\)](../WarehouseActivities/-$-n_900-assembly-order-$-.md)   
 [\($ T\_90\_20 Resource Usage Type $\)](../Topic/\($%20T_90_20%20Resource%20Usage%20Type%20$\).md)   
 [How to: Assemble Items](../WarehouseActivities/how-to-assemble-items.md)   
 [Assembly BOMs or Production BOMs](../DesignAndEngineering/assembly-boms-or-production-boms.md)   
 [How to: Calculate the Standard Cost of Assembly BOMs](../Finance/how-to-calculate-the-standard-cost-of-assembly-boms.md)   
 [How to: Explode Assembly BOMs](../DesignAndEngineering/how-to-explode-assembly-boms.md)   
 [How to: Run MPS and MRP](../OperationsPlanning/how-to-run-mps-and-mrp.md)