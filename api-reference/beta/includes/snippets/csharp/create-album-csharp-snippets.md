---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 08f9e6f5d2228157c4c4deaa4dfc010b98f7df7c36c563e82d3cd796859fc9b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57195515"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "My Day at the Beach",
    Bundle = new Bundle
    {
        Album = new Album
        {
        }
    },
    Children = new DriveItemChildrenCollectionPage()
    {
        new DriveItem
        {
            Id = "1234asdf"
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"@microsoft.graph.conflictBehavior", "rename"}
    }
};

await graphClient.Drive.Bundles
    .Request()
    .AddAsync(driveItem);

```