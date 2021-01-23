---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a3cd18c65d0684b4297a7b8d45868becc81e09fd
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var list = new List
{
    DisplayName = "Books",
    Columns = new ListColumnsCollectionPage()
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