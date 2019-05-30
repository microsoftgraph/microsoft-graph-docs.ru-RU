---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 470c49291b9731789cdff260e9deb2ccf6377450
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new SynchronizationJobRestartCriteria
{
    ResetScope = SynchronizationJobRestartScope.QuarantineState | SynchronizationJobRestartScope.Escrows | SynchronizationJobRestartScope.ConnectorDataStore
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Restart(criteria)
    .Request()
    .Header("Authorization","Bearer <token>")
    .PostAsync();

```