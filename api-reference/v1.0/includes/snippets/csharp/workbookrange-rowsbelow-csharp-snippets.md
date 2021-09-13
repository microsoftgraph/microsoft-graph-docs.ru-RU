---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c587c2104274f7dec5a9bc2e06c78c10bb0d349743593165e42ffb22ec760c10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57264552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .RowsBelow(2)
    .Request()
    .GetAsync();

```