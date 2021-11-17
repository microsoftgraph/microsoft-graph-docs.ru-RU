---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc5b6bff5ead6722e745152108484b69eaabcfb3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995062"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAuthorizationPolicy()
blockMsolPowerShell := true
requestBody.SetBlockMsolPowerShell(&blockMsolPowerShell)
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
authorizationPolicyId := "authorizationPolicy-id"
graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```