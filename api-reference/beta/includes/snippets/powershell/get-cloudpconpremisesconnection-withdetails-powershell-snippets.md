---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 58d70f2f1ebfcc83aaec54f1854e66f85ab84fa4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109321"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointOnPremisesConnection -CloudPcOnPremisesConnectionId $cloudPcOnPremisesConnectionId -Property "id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse" 

```