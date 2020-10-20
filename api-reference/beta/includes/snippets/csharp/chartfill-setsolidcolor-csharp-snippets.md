---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 65cf70a7b0b2277e217ba9857f0806c2f8c8822b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616824"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var color = "color-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Format.Fill
    .SetSolidColor(color)
    .Request()
    .PostAsync();

```