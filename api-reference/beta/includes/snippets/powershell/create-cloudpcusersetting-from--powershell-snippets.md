---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5348b83d8cdb25eced3dffef009e141c8ff8393f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126587"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcUserSetting"
    DisplayName = "Example"
    SelfServiceEnabled = $false
    LocalAdminEnabled = $true
}

New-MgDeviceManagementVirtualEndpointUserSetting -BodyParameter $params

```