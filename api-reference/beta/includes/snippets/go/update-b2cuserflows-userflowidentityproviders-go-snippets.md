---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2368cab7fb53d00833b0c6a35b6e6f22ae6375ca
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342582"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}",
    "@odata.type": "#microsoft.graph.identityProvider",
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
identityProviderBaseId := "identityProviderBase-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserFlowIdentityProvidersById(&identityProviderBaseId).Patch(requestBody)


```