---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4da83fe3d1587724b1a59e1595cc9ccd83127c51
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589303"
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
    IsOrganizationDefault = true
};

await graphClient.Policies.TokenLifetimePolicies
    .Request()
    .AddAsync(tokenLifetimePolicy);

```