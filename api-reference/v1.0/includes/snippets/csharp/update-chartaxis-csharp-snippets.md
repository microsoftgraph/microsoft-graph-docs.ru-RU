---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a42711849bd3b5b3777cd52cb2e23551f8bd752c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = JToken.Parse("{}"),
    Maximum = JToken.Parse("{}"),
    Minimum = JToken.Parse("{}")
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```