---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4770f401e240f1236158df5e34f21e1f7f19a712
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsBelow(null)
    .Request()
    .PostAsync();

```