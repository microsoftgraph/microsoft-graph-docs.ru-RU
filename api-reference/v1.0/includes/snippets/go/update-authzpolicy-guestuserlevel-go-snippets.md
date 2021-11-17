---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 657a7ba531fe4cd598307a7a2b84174434285323
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001338"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAuthorizationPolicy()
allowEmailVerifiedUsersToJoinOrganization := false
requestBody.SetAllowEmailVerifiedUsersToJoinOrganization(&allowEmailVerifiedUsersToJoinOrganization)
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().AuthorizationPolicy().Patch(options)


```