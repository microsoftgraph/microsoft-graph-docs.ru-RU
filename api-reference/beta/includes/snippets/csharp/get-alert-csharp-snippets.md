---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d4df16ee11685a1b4d429214ba577f4c26eef537
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622100"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{id}"]
    .Request()
    .GetAsync();

```