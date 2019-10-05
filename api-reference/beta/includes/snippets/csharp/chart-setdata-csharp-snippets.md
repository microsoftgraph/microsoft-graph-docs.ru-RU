---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c439647a3b1e46fc1f0facf8dc40405c108a5558
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceData = "sourceData-value";

var seriesBy = "seriesBy-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .SetData(seriesBy,sourceData)
    .Request()
    .PostAsync();

```