---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44fa7dbc50e4a514f49e798ee2b54314e2327256
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentials = new List<SynchronizationSecretKeyStringValuePair>()
{
    new SynchronizationSecretKeyStringValuePair
    {
    }
};

await graphClient.Applications["{application-id}"].Synchronization
    .AcquireAccessToken(credentials)
    .Request()
    .PostAsync();

```