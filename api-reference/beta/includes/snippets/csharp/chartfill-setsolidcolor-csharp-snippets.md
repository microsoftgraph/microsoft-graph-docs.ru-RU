---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: edbb00e6e3f50caa9d6b4f447cf41bd7571d0f68
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var color = "color-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Format.Fill
    .SetSolidColor(color)
    .Request()
    .PostAsync();

```