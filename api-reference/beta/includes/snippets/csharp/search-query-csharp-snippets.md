---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a27130770eb1291d67d18c6435906b3cc5a44ad4
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var requests = new List<SearchRequestObject>()
{
    new SearchRequestObject
    {
        EntityTypes = new List<EntityType>()
        {
            EntityType.ExternalItem
        },
        ContentSources = new List<String>()
        {
            "/external/connections/connectionfriendlyname"
        },
        Query = new SearchQuery
        {
            Query_string = new SearchQueryString
            {
                Query = "contoso product"
            }
        },
        From = 0,
        Size = 25,
        Stored_fields = new List<String>()
        {
            "title",
            "description"
        }
    }
};

await graphClient.Search
    .Query(requests)
    .Request()
    .PostAsync();

```