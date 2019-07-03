---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0e60d1d547ea8bbf50615c0cf7b907d3142e14a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = new Json
    {
    },
    Maximum = new Json
    {
    },
    Minimum = new Json
    {
    }
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```