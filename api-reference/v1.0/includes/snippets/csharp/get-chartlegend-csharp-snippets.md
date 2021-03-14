---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c65717152f0e80b2bcbe15a832878dcf52bc20b5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartLegend = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Legend
    .Request()
    .GetAsync();

```