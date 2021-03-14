---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8efecdc137188f8a3cccdba7a4fc971b764ea957
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .UsedRange(true)
    .Request()
    .GetAsync();

```