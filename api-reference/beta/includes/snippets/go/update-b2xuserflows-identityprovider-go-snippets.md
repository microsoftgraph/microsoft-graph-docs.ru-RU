---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96c506ecf9b79947878814bf869d73d2f714fbee
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341211"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}",
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
identityProviderId := "identityProvider-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).IdentityProvidersById(&identityProviderId).Post(requestBody)


```