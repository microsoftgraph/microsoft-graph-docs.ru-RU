---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d98b01bceb2afa08c9f6c84ae8f531c0d4f104d
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "New Folder",
    Folder = new Folder
    {
    },
    @microsoft.graph.conflictBehavior = "rename"
};

await graphClient.Me.Drive.Root.Children
    .Request()
    .AddAsync(driveItem);

```