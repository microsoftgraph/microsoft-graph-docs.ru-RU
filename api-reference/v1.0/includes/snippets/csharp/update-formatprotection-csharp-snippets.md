---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ed57caea3b70bb1d211b3b71bc28c03313f5195eb4c79973b6f0fa392dbcc3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255092"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = new WorkbookFormatProtection
{
    Locked = true,
    FormulaHidden = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Protection
    .Request()
    .UpdateAsync(workbookFormatProtection);

```