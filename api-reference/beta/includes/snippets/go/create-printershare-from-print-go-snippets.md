---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c163e2fe7dead23d811dabb068bea634c6292db5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrinterShare()
name := "name-value"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}",
}
options := &msgraphsdk.SharesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Print().Shares().Post(options)


```