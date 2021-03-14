---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b764c8d2e5183f3bce56e7426038fd282ce6d65
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.SeriesAxis.Format.Line
    .Clear()
    .Request()
    .PostAsync();

```