---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: da8e2dd32d1ad4b185f440258064b4915d93f45b
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var contacts = await graphClient.Contacts
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName,'A')")
    .OrderBy("displayName")
    .Top(1)
    .GetAsync();

```