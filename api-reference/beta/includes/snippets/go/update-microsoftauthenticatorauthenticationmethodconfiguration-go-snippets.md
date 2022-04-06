---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bde1c71a83b6f865b08c7e2ad932b1ea58cd359a
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528800"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationMethodConfiguration()
state := "String"
requestBody.SetState(&state)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
}
options := &msgraphsdk.AuthenticationMethodConfigurationRequestBuilderPatchOptions{
    Body: requestBody,
}
authenticationMethodConfigurationId := "authenticationMethodConfiguration-id"
graphClient.Policies().AuthenticationMethodsPolicy().AuthenticationMethodConfigurationsById(&authenticationMethodConfigurationId).Patch(options)


```