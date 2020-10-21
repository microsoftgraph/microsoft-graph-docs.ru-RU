---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e0984a84a80c562a3635df91130665d05c7b9566
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{alert_id}"]
    .Request()
    .GetAsync();

```