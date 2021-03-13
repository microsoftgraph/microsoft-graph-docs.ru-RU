---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96e6352f8c6fedb2ff85518100eb7ee331b0acd1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOnPremisesConnection = await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{cloudPcOnPremisesConnection-id}"]
    .Request()
    .GetAsync();

```