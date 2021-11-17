---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f8563329f91e6ab8f854dafa249884b98e2ca9d6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025136"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrinterShare()
displayName := "ShareName"
requestBody.SetDisplayName(&displayName)
allowAllUsers := false
requestBody.SetAllowAllUsers(&allowAllUsers)
requestBody.SetAdditionalData(map[string]interface{}{
    "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}",
}
options := &msgraphsdk.SharesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Print().Shares().Post(options)


```