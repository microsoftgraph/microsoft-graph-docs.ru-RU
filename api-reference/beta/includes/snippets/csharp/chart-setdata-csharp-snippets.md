---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cda230c0c686251a67fb531830c94e5be72ba574
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceData = "sourceData-value";

var seriesBy = "seriesBy-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"]
    .SetData(seriesBy,sourceData)
    .Request()
    .PostAsync();

```