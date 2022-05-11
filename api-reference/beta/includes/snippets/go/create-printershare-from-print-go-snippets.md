---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1618c2a3205a9f48a94ac9d5d271542ee0ae4d5a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340838"
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
result, err := graphClient.Print().Shares().Post(requestBody)


```