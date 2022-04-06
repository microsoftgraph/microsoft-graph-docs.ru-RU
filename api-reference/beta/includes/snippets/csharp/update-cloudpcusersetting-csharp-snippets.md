---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d248f2d11d06bd9d28bc33603189edd0bccfdb4
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcUserSetting = new CloudPcUserSetting
{
    DisplayName = "Example",
    SelfServiceEnabled = true,
    RestorePointSetting = new CloudPcRestorePointSetting
    {
        FrequencyInHours = 16,
        UserRestoreEnabled = true
    },
    LocalAdminEnabled = false
};

await graphClient.DeviceManagement.VirtualEndpoint.UserSettings["{cloudPcUserSetting-id}"]
    .Request()
    .UpdateAsync(cloudPcUserSetting);

```