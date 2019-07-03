---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c1cf0ff945b7cb8050572077fe78716ad18e514
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    ParentReference = new ItemReference
    {
        Id = "new-parent-folder-id"
    },
    Name = "new-item-name.txt"
};

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .UpdateAsync(driveItem);

```