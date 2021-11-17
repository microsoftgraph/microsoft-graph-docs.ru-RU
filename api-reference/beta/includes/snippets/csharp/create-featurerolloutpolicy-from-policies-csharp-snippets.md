---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7339ca5ecd6f3556825f129aca18eab11c421d4d4f1736154715682e02f481af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = new FeatureRolloutPolicy
{
    DisplayName = "PassthroughAuthentication rollout policy",
    Description = "PassthroughAuthentication rollout policy",
    Feature = StagedFeatureName.PassthroughAuthentication,
    IsEnabled = true,
    IsAppliedToOrganization = false
};

await graphClient.Policies.FeatureRolloutPolicies
    .Request()
    .AddAsync(featureRolloutPolicy);

```