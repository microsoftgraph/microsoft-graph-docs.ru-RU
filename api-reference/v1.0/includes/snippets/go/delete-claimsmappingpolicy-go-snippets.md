---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e419640c4188344e6d2f2f1e67e33645ac7678a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091234"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

claimsMappingPolicyId := "claimsMappingPolicy-id"
graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Delete(options)


```