---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c5cb691f40b3861c8a1f3ad4320c51f5ee342f0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition
{
    AttributeSet = "Engineering",
    Description = "Target completion date",
    IsCollection = false,
    IsSearchable = true,
    Name = "ProjectDate",
    Status = "Available",
    Type = "String",
    UsePreDefinedValuesOnly = false
};

await graphClient.Directory.CustomSecurityAttributeDefinitions
    .Request()
    .AddAsync(customSecurityAttributeDefinition);

```