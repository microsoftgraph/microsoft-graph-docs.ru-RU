---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 72520adae193e0ab3182c33c1b438e3a8986454f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var password = "password-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Unprotect()
    .Request()
    .PostAsync();

```