---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 90cc7f62eee42c40d93732549f52e9dc0a877982
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983982"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrintTaskTrigger()
event := "jobStarted"
requestBody.SetEvent(&event)
requestBody.SetAdditionalData(map[string]interface{}{
    "definition@odata.bind": "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}",
}
options := &msgraphsdk.TaskTriggersRequestBuilderPostOptions{
    Body: requestBody,
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggers().Post(options)


```