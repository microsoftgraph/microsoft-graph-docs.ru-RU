---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 864646a6ff04e2002c4c182834b678327137fe42
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800048"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables["{workbookPivotTable-id}"]
    .Request()
    .GetAsync();

```