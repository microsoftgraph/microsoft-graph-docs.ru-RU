---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fc368d656c4daeab14af8c208849c8728b1e9cf
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342094"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
}
headers := map[string]string{
    "Authorization": "Bearer <token>"
}
options := &msgraphsdk.SynchronizationTemplateRequestBuilderPutRequestConfiguration{
    Headers: headers,
}
applicationId := "application-id"
synchronizationTemplateId := "synchronizationTemplate-id"
graphClient.ApplicationsById(&applicationId).Synchronization().TemplatesById(&synchronizationTemplateId).PutWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```