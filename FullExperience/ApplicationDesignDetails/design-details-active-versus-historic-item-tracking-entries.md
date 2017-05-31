---
title: "Design Details: Active versus Historic Item Tracking Entries"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "item tracking, active vs. historic"
ms.assetid: 587ca5d0-2fe5-462e-906b-883b5a578799
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
# Design Details: Active versus Historic Item Tracking Entries
When parts of a document line quantity are posted, only that particular quantity is transferred to the item ledger entries and its item tracking numbers. However, you will want to access all relevant item tracking information directly from the active document line. That is, not only will you want to see the entries that are related to the remaining quantity, you will also want information about the units that have been posted. When you view or modify the **Item Tracking Lines** window, the collective contents of the **Tracking Specification** table \(T336\) and **Reservation Entry** table \(T337\) are presented in a temporary version of T336. This ensures that historic and active item tracking data is accessed as one.  
  
 The following table shows how T336 and T337 are used in a purchase scenario. The bold figures represent values that the user manually enters in the **\($ N\_6510 Item Tracking Lines $\)** window.  
  
 Step 1: Create a purchase order line of seven pieces with item tracking numbers.  
  
||**\($ T\_6550\_4 Quantity \(Base\) $\)**|**\($ T\_6550\_60 Qty. to Handle $\)**|**\($ T\_6550\_51 Qty. to Invoice \(Base\) $\)**|**\($ T\_6550\_52 Quantity Handled \(Base\) $\)**|**\($ T\_6550\_53 Quantity Invoiced \(Base\) $\)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**T337**|7|0|0|0|0|  
|**T336**|0|0|0|0|0|  
  
 Step 2: Receive four pieces.  
  
||**\($ T\_6550\_4 Quantity \(Base\) $\)**|**\($ T\_6550\_60 Qty. to Handle $\)**|**\($ T\_6550\_51 Qty. to Invoice \(Base\) $\)**|**\($ T\_6550\_52 Quantity Handled \(Base\) $\)**|**\($ T\_6550\_53 Quantity Invoiced \(Base\) $\)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|7|**4**|**0**|0|0|  
|**T337**|3|0|0|0|0|  
|**T336**|4|0|0|4|0|  
  
 Step 3: Receive two pieces and invoice two pieces.  
  
||**\($ T\_6550\_4 Quantity \(Base\) $\)**|**\($ T\_6550\_60 Qty. to Handle $\)**|**\($ T\_6550\_51 Qty. to Invoice \(Base\) $\)**|**\($ T\_6550\_52 Quantity Handled \(Base\) $\)**|**\($ T\_6550\_53 Quantity Invoiced \(Base\) $\)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|7|**2**|**2**|4|0|  
|**T337**|1|0|0|0|0|  
|**T336**|6|0|0|6|2|  
  
 Step 4: Receive one piece.  
  
||**\($ T\_6550\_4 Quantity \(Base\) $\)**|**\($ T\_6550\_60 Qty. to Handle $\)**|**\($ T\_6550\_51 Qty. to Invoice \(Base\) $\)**|**\($ T\_6550\_52 Quantity Handled \(Base\) $\)**|**\($ T\_6550\_53 Quantity Invoiced \(Base\) $\)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|7|**1**|**0**|6|2|  
|**T336**|7|0|0|7|2|  
  
 Invoice 5 pieces.  
  
||**\($ T\_6550\_4 Quantity \(Base\) $\)**|**\($ T\_6550\_60 Qty. to Handle $\)**|**\($ T\_6550\_51 Qty. to Invoice \(Base\) $\)**|**\($ T\_6550\_52 Quantity Handled \(Base\) $\)**|**\($ T\_6550\_53 Quantity Invoiced \(Base\) $\)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|7|0|**5**|7|2|  
|**T336**|7|0|0|7|7|  
  
## See Also  
 [Design Details: Item Tracking](../ApplicationDesign/design-details-item-tracking.md)   
 [Design Details: Item Tracking Lines Window](../ApplicationDesign/design-details-item-tracking-lines-window.md)