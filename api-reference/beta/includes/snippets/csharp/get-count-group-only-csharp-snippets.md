---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0a306236b3aa6401e4d6dfa03ad354113a27c73e
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.ServicePrincipals["{id}"].MemberOf.Microsoft.graph.group.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```