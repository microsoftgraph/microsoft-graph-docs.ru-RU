---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6cf4b1070c3435a626d8162892d7d96dcbf1b24bbd3e9333fed2776d8b5eca70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57369334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "fields")
};

var listItem = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"]
    .Request( queryOptions )
    .GetAsync();

```