---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dcd48e0656bdcbbed4eed9da893f136655211ae74ba65fc7bf3dffc7a7e649d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322532"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = new FeatureRolloutPolicy();
featureRolloutPolicy.displayName = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.description = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.feature = StagedFeatureName.PASSTHROUGH_AUTHENTICATION;
featureRolloutPolicy.isEnabled = true;
featureRolloutPolicy.isAppliedToOrganization = false;

graphClient.policies().featureRolloutPolicies()
    .buildRequest()
    .post(featureRolloutPolicy);

```