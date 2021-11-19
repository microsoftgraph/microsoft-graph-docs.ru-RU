---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f2636ba1c77e921aa422ba3c8e627f197bcafed7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086208"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

featureRolloutPolicyId := "featureRolloutPolicy-id"
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Delete(options)


```