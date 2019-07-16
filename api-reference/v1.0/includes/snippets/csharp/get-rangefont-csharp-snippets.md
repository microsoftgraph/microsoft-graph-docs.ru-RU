---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb45e3738300a3171aa2cbd81ec8dfab3cded157
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735513"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Font
    .Request()
    .GetAsync();

```