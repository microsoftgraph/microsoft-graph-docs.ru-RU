---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 760dda536d9e37cb677c780524f79d1ee61cd00e3d8702aa4fd246632add7833
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050387"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartSeries = new WorkbookChartSeries
{
    Name = "name-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Series
    .Request()
    .AddAsync(workbookChartSeries);

```