---
title: "How to: Use Event Viewer to Collect and View Trace Events"
ms.custom: na
ms.date: 04/01/2021
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: conceptual
ms.assetid: ddd157e5-069a-44c5-b25b-1e90cb0bf1d0
caps.latest.revision: 4
author: SusanneWindfeldPedersen
---
# Enable Business Central Debug Logs in Event Viewer

Some [!INCLUDE[server](../developer/includes/server.md)] events are collected in the following **Debug** logs specific to [!INCLUDE[prod_short](../developer/includes/prod_short.md)] in Event Viewer:

-   **Applications and Services Logs** > **Microsoft** > **DynamicsNAV** > **Server**

- **Applications and Services Logs** > **Microsoft** > **DynamicsNAV** > **Common**

By default the **Debug** logs are disabled and may also be hidden in the Event Viewer. To collect trace event data, you must enable the **Debug** logs.  
  
### To enable Debug logs in Event Viewer  
  
1.  On the computer that is running [!INCLUDE[server](../developer/includes/server.md)], start Event Viewer.  
  
     For more information, see [How to Start Event Viewer](/previous-versions/).  
  
2.  In the console tree, choose **Applications and Services Logs**, **Microsoft**, **DynamicsNAV**, and then **Server** or **Common**.  
  
3.  If the **Debug** log is not shown under **Server**, then on the **View** menu, select **Show Analytic and Debug Logs**.  
  
4.  Select the **Debug** log, and then on the **Actions** menu, choose **Enable Log**.  
  
    > [!NOTE]  
    >  Depending on the number of events, you might have to increase the maximum size of the log. The default value is 1028 KB. For more information, see [Set Maximum Log Size](/previous-versions/windows/it-pro/windows-server-2008-R2-and-2008/cc748849(v=ws.11)).  
  
 [!INCLUDE[server](../developer/includes/server.md)] trace events will now be recorded in the **Debug** log. For a list and description of trace events, see [Business Central Server Trace Events](server-trace-events.md).  
  
## See Also  
 [Monitoring Business Central Server Events](monitor-server-events.md)    
 [Show or Hide Analytic and Debug](/previous-versions/windows/it-pro/windows-server-2008-R2-and-2008/cc766275(v=ws.11))   
 [Enable Analytic and Debug Logs](/previous-versions/windows/it-pro/windows-server-2008-R2-and-2008/cc749492(v=ws.11))