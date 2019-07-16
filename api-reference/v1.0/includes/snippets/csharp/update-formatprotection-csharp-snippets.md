---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d98fc1317500d7342fd99fe930198b50a11e862
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740232"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = new WorkbookFormatProtection
{
    Locked = true,
    FormulaHidden = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Protection
    .Request()
    .UpdateAsync(workbookFormatProtection);

```