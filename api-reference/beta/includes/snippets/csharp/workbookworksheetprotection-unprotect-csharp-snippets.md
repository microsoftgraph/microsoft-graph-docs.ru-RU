---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 72520adae193e0ab3182c33c1b438e3a8986454f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var password = "password-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Unprotect()
    .Request()
    .PostAsync();

```