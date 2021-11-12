---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f8142e6435aeda82aa4242de5f1eb9c193283183b53ab37ab75322c8f72e2af3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = JsonDocument.Parse("{}"),
    Maximum = JsonDocument.Parse("{}"),
    Minimum = JsonDocument.Parse("{}")
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```