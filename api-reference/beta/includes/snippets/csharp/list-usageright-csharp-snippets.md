---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b1576d7ea0bff6c41675caaa0d076529a0b6c6b0
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Users["{userId}"].UsageRights
    .Request()
    .Filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .GetAsync();

```