---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 727c044502df9ab5b0e74ff1f7fa3a6e47eabe81
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "name,lastModifiedDateTime"),
    new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))")
};

var list = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
    .Request( queryOptions )
    .GetAsync();

```