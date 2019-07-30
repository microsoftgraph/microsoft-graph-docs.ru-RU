---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6339e7382bd820b347218c6349534adaa9fcdea8
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "Just some files",
    @name.conflictBehavior = "rename",
    Bundle = new Bundle
    {
    },
    Children = new List<DriveItem>()
    {
        new DriveItem
        {
            Id = "1234asdf"
        },
        new DriveItem
        {
            Id = "1234qwerty"
        }
    }
};

await graphClient.Drive.Bundles
    .Request()
    .AddAsync(driveItem);

```