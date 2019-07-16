---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 528fe4d0195b56e54c7f3b07fec03be57ef701d7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartGridlines = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.MinorGridlines
    .Request()
    .GetAsync();

```