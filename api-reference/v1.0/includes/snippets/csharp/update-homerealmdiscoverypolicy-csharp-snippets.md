---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 21d2a802f183cb6ea85d0098e1fcff6d77875c1b
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.HomeRealmDiscoveryPolicies["{id}"]
    .Request()
    .UpdateAsync(homeRealmDiscoveryPolicy);

```