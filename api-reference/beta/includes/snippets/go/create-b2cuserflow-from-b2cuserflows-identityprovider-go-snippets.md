---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: daa39ebe27928d4f6c1c6e9f2167dee35ba40fa9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102627"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2cIdentityUserFlow()
id := "Customer"
requestBody.SetId(&id)
userFlowType := "signUpOrSignIn"
requestBody.SetUserFlowType(&userFlowType)
userFlowTypeVersion := float32(3)
requestBody.SetUserFlowTypeVersion(&userFlowTypeVersion)
requestBody.SetIdentityProviders( []IdentityProvider {
    msgraphsdk.NewIdentityProvider(),
    SetAdditionalData(map[string]interface{}{
        "id": "Facebook-OAuth",
    }
}
headers := map[string]string{
    "Location": "https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')"
}
options := &msgraphsdk.B2cUserFlowsRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.Identity().B2cUserFlows().Post(options)


```