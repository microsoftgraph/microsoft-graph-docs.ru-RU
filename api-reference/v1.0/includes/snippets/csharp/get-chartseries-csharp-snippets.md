---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 89d0384c829fd45e09c7ac97a7765255f600ed58d52ffb0ae414aea37350c2a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57259326"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartSeries = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Series["{workbookChartSeries-id}"]
    .Request()
    .GetAsync();

```