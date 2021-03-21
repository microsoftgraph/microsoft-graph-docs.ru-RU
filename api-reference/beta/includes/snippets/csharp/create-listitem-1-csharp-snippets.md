---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d93bef0bf2e3a4396f11a5ec3512bf9bc078806c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var listItem = new ListItem
{
    Fields = new FieldValueSet
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"Title", "Widget"},
            {"Color", "Purple"},
            {"Weight", "32"}
        }
    }
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
    .Request()
    .AddAsync(listItem);

```