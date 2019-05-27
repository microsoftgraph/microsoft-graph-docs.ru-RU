---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e1c06f46014b8e1afc72fd6306a9dab8a82e62d2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeBorder = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Borders["{sideIndex}"]
    .Request()
    .GetAsync();

```