---
title: "How to: Calculate Bin Replenishment"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "replenishing pick bins"
  - "bins, calculating replenishment"
ms.assetid: 48fa5f81-ce8a-42d8-9179-660a23385959
caps.latest.revision: 8
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
# How to: Calculate Bin Replenishment
When the location is set up to use directed put\-away and pick, priorities of the put\-away template for the location are taken into account when putting receipts away. Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings. Therefore, if items are arriving at a steady pace, the most\-used pick bins will be filled up as they are emptied.  
  
 But inventory does not always arrive in a steady trickle. Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost. Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.  
  
 It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.  
  
 Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away\-type bins are not suggested for a pick of inventory.  
  
### To replenish pick bins  
  
1.  In the **Search** box, enter **\($ N\_7351 Movement Worksheet $\)**, and then choose the related link.  
  
2.  On the **Actions** tab, in the **Functions** group, Choose **\($ B\_7300 Calculate Bin Replenishment $\)** to open the report request page.  
  
3.  Fill in the batch job request window to limit the scope of the replenishment suggestions that will be calculated. For example, you might be concerned with particular items, zones, or bins.  
  
4.  Choose the **OK** button. Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.  
  
5.  If you want to perform all the suggested replenishments, on the **Actions** tab, in the **Functions** group, choose **Create Movement.** Employees can now find instructions in the **Movements** menu item, carry them out and register them.  
  
6.  If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.  
  
     The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.  
  
> [!NOTE]  
>  If the following conditions are met for an item:  
>   
>  -   The item has an expiration date, and  
> -   The **Pick According to FEFO** field on the location card is selected, and  
> -   You use the **Calculate Bin Replenishment** functionality  
>   
>  then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.  
  
## See Also  
 [\($ B\_7300 Calculate Bin Replenishment $\)](../Topic/\($%20B_7300%20Calculate%20Bin%20Replenishment%20$\).md)   
 [\($ N\_7351 Movement Worksheet $\)](../Topic/\($%20N_7351%20Movement%20Worksheet%20$\).md)   
 [Move Items](../WarehouseActivities/move-items.md)   
 [Design Details: Internal Warehouse Flows](../ApplicationDesign/design-details-internal-warehouse-flows.md)