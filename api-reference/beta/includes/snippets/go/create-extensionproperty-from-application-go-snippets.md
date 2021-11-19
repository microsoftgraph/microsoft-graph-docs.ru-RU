---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 130f5decb750f538d99c9fa9852262fb4cf92237
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095376"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExtensionProperty()
name := "extensionName"
requestBody.SetName(&name)
dataType := "string"
requestBody.SetDataType(&dataType)
requestBody.SetTargetObjects( []String {
    "Application",
}
options := &msgraphsdk.ExtensionPropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).ExtensionProperties().Post(options)


```