---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c3d9aa2d3319041c2c3665d314bdea8d0a7f93b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printIdentity = new PrintIdentity
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/groups/{id}"}
    }
};

await graphClient.Print.Shares["{id}"].AllowedGroups.References
    .Request()
    .AddAsync(printIdentity);

```