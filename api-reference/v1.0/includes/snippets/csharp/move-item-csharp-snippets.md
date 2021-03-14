---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: efda284db12a5cee6ba6ee47e240a0d2200822a6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803771"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    ParentReference = new ItemReference
    {
        Id = "{new-parent-folder-id}"
    },
    Name = "new-item-name.txt"
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Request()
    .UpdateAsync(driveItem);

```