---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1015b0547df389e35fbfa683b8cff48aeee077df
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var list = new List
{
    DisplayName = "Books",
    Columns = (IListColumnsCollectionPage)new List<ColumnDefinition>()
    {
        new ColumnDefinition
        {
            Name = "Author",
            Text = new TextColumn
            {
            }
        },
        new ColumnDefinition
        {
            Name = "PageCount",
            Number = new NumberColumn
            {
            }
        }
    },
    ListInfo = new ListInfo
    {
        Template = "genericList"
    }
};

await graphClient.Sites["{site-id}"].Lists
    .Request()
    .AddAsync(list);

```