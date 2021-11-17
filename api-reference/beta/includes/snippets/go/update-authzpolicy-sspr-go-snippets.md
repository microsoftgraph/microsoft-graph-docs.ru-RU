---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fa17b35cfc8970878985269ed7e919c584bfbca7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995059"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAuthorizationPolicy()
allowedToUseSSPR := true
requestBody.SetAllowedToUseSSPR(&allowedToUseSSPR)
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
authorizationPolicyId := "authorizationPolicy-id"
graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```