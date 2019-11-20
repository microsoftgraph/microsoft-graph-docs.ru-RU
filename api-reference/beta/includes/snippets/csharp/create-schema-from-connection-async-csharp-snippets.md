---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 19a2315ff73d1bd0cd8f3696e612b756c689e79d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995510"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = new Schema
{
    BaseType = "microsoft.graph.externalItem",
    Properties = new List<Property>()
    {
        new Property
        {
            Name = "title",
            Type = PropertyType.String,
            IsSearchable = true,
            IsRetrievable = true
        },
        new Property
        {
            Name = "priority",
            Type = PropertyType.String,
            IsQueryable = true,
            IsRetrievable = true
        },
        new Property
        {
            Name = "assignee",
            Type = PropertyType.String,
            IsRetrievable = true
        }
    }
};

await graphClient.Connections["contosohr"].Schema
    .Request()
    .Header("Prefer","respond-async")
    .AddAsync(schema);

```