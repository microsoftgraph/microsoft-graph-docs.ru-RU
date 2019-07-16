---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ed287f9a72ee639e8b79b00e2ac0f2be2904154
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var points = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{series-id}"].Points
    .Request()
    .GetAsync();

```