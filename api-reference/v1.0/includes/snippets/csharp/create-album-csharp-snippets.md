---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3084bbd1bcbd61d373296c01cd0566a6b7954d5a
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757710"
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