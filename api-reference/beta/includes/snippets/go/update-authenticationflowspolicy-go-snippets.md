---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fc08bd289070b920204896dfae0c80a212857fe5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982336"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAuthenticationFlowsPolicy()
selfServiceSignUp := msgraphsdk.NewSelfServiceSignUpAuthenticationFlowConfiguration()
requestBody.SetSelfServiceSignUp(selfServiceSignUp)
isEnabled := true
selfServiceSignUp.SetIsEnabled(&isEnabled)
options := &msgraphsdk.AuthenticationFlowsPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().AuthenticationFlowsPolicy().Patch(options)


```