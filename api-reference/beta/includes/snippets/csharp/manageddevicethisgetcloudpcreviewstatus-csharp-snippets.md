---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dca8946fd67adde37fc9fb8e02119a93f8d5b633
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694579"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcReviewStatus = await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .GetCloudPcReviewStatus()
    .Request()
    .GetAsync();

```