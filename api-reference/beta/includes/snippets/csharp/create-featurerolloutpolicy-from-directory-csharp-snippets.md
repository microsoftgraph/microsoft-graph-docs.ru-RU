---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b4a5a47ed27290a774d02a3c398213e77865578e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172976"
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

await graphClient.Directory.FeatureRolloutPolicies
    .Request()
    .AddAsync(featureRolloutPolicy);

```