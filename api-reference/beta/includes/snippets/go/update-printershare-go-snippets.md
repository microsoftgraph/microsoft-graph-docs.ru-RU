---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 58fbd4c53b43d6bb47e404e25e2a54159aa3d746
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028040"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrinterShare()
displayName := "ShareName"
requestBody.SetDisplayName(&displayName)
allowAllUsers := true
requestBody.SetAllowAllUsers(&allowAllUsers)
requestBody.SetAdditionalData(map[string]interface{}{
    "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}",
}
options := &msgraphsdk.PrinterShareRequestBuilderPatchOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
graphClient.Print().SharesById(&printerShareId).Patch(options)


```