---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 019425ff86e2b172c692fd8efd6c84b937dcea82
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterOperators = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema.FilterOperators()
    .Request()
    .GetAsync();

```