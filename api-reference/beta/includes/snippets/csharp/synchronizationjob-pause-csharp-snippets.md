---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 975c83c236713dacca1fe4f100cdd9a6378f33da
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Pause()
    .Request()
    .PostAsync();

```