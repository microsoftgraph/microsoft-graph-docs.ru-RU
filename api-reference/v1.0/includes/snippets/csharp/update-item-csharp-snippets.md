---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 75ed18f3bcd9040af90ae6e9686f61aac70b75da1ac9b573b7122d180ffe924f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57325238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "new-file-name.docx"
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Request()
    .UpdateAsync(driveItem);

```