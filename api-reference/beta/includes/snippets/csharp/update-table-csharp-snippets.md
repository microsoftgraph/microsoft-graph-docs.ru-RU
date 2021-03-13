---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a02ac3ce357f3e2fd18559c5b18ce2179018c0a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTable = new WorkbookTable
{
    Name = "name-value",
    ShowHeaders = true,
    ShowTotals = true,
    Style = "style-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Request()
    .UpdateAsync(workbookTable);

```