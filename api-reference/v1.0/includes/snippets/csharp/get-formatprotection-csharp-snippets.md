---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a7f7a86f9cafa2386f50f6875ad3a9fb3de5f92c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Protection
    .Request()
    .GetAsync();

```