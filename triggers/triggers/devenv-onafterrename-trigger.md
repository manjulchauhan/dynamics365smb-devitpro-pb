---
title: "OnAfterRename Trigger"
description: "OnAfterRename trigger in AL for Business Central."
ms.custom: na
ms.date: 04/01/2021
ms.reviewer: solsen
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: reference
ms.author: t-blrobl
author: blrobl
---

# OnAfterRename Trigger
Runs when a user tries to rename a record.  

## Applies to  
- Table extensions 
  
## Remarks  
When you rename a record in one location, it is updated in all other locations. It runs automatically when the user changes a record's primary key field in a page from the Web Client.  The OnBeforeRename trigger runs after field validation and after the default renaming behavior, which checks that the new name does not correspond to an already existing record before the rename occurs. The record is not renamed if an error occurs in the trigger code.  

## See Also  
 [Triggers](devenv-triggers.md)  
 [Table and Field Triggers](devenv-table-and-field-triggers.md)  
 [OnBeforeRename Trigger](devenv-onbeforerename-trigger.md)    