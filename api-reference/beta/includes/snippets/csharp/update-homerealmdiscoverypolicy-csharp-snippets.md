---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 30505b1e920cd2b34e7cec615d7223d44cc20520
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy
{
    Definition = new List<String>()
    {
        "{\"HomeRealmDiscoveryPolicy\":\r\n     {\"AccelerateToFederatedDomain\":true,\r\n      \"PreferredDomain\":\"federated.example.edu\",\r\n      \"AlternateIdLogin\":{\"Enabled\":true}}}"
    },
    DisplayName = "Contoso default HRD Policy"
};

await graphClient.Policies.HomeRealmDiscoveryPolicies["{homeRealmDiscoveryPolicy-id}"]
    .Request()
    .UpdateAsync(homeRealmDiscoveryPolicy);

```