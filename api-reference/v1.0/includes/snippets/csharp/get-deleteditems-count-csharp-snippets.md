---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: df8e1604ae551f451d22779028af5efb0b7ebd9d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var group = await graphClient.Directory.DeletedItems
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Select("id,displayName,deletedDateTime")
    .OrderBy("deletedDateTime asc")
    .GetAsync();

```