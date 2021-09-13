---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a484973ef51a797b36ec0d2d72cfa7286c26849883e72ebd505fbc8e1755371c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxisTitle = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis.Title
    .Request()
    .GetAsync();

```