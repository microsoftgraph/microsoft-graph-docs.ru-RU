---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31fb531b04f2fa325cf537a3ab86e1c976e61eab
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528733"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcUserSetting"
    DisplayName = "Example"
    SelfServiceEnabled = $true
    RestorePointSetting = @{
        FrequencyInHours = 16
        UserRestoreEnabled = $true
    }
    LocalAdminEnabled = $false
}

Update-MgDeviceManagementVirtualEndpointUserSetting -CloudPcUserSettingId $cloudPcUserSettingId -BodyParameter $params

```