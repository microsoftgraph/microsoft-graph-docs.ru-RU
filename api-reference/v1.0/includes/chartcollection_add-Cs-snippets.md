---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b5739ae3ab82a5a0e90636205ce2fc12f66cea6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469197"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "ColumnStacked";

var sourceData = "A1:B1";

var seriesBy = "Auto";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts
    .Add(type,sourceData,seriesBy)
    .Request()
    .PostAsync();

```