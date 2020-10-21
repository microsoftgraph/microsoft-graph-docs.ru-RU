---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc23ce61c9a64e1474d25d8c0a4036eba7f48671
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Request()
    .GetAsync();

```