---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 331f0543c999d5eff2351644a88161d80361e944
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59766801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCloudPcRemoteActionResults = await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .GetCloudPcRemoteActionResults()
    .Request()
    .GetAsync();

```