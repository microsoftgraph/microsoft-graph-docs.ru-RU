---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d7427ff6090c783ff42a35c115fcaf00f7055c0
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589278"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = new TokenLifetimePolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true,
    Type = "type-value"
};

await graphClient.Policies.TokenLifetimePolicies["{id}"]
    .Request()
    .UpdateAsync(tokenLifetimePolicy);

```