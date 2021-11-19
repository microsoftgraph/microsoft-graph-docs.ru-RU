---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a0ffa86e3df8cc1cef99c6888d722680866265d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test",
    "@odata.type": "#microsoft.graph.identityProvider",
}
options := &msgraphsdk.RefRequestBuilderPatchOptions{
    Body: requestBody,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserFlowIdentityProviders().$ref().Patch(options)


```