---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 791de5ca8bec051eb4cfbeb0f5a1723929caa2b1
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508369"
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