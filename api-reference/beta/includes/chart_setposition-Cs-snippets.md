---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: de7c2feea618ecf6f3d8b86eb357d3282e4e03e2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var startCell = "startCell-value";

var endCell = "endCell-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .SetPosition(startCell,endCell)
    .Request()
    .PostAsync();

```