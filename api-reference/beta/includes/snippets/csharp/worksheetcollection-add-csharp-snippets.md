---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3a495bc94ddafdbddafd33f106c65c49410ea32d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723577"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "name-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets
    .Add(name)
    .Request()
    .PostAsync();

```