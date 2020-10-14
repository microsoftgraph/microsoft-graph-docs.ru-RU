---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5aaf99426bd9ebfed65a0c5ff5bc4e9a0e91700e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = new Microsoft.Graph.TermStore.Term
{
    Labels = new List<Microsoft.Graph.TermStore.LocalizedLabel>()
    {
        new Microsoft.Graph.TermStore.LocalizedLabel
        {
            LanguageTag = "en-US",
            Name = "Car",
            IsDefault = true
        }
    }
};

await graphClient.TermStore.Sets["{setId}"].Terms
    .Request()
    .AddAsync(term);

```