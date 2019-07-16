---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 65cf70a7b0b2277e217ba9857f0806c2f8c8822b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var color = "color-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Format.Fill
    .SetSolidColor(color)
    .Request()
    .PostAsync();

```