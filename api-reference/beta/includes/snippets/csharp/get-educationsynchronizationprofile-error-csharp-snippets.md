---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1109d0b032d38cb7400ed5160f419dd4b98eed93
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714436"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var errors = await graphClient.Education.SynchronizationProfiles["{id}"].Errors
    .Request()
    .GetAsync();

```