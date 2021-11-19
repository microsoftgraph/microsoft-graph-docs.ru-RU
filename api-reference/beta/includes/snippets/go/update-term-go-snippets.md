---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7191a032653319774f3230c115dbf854536917d1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092867"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
    SetAdditionalData(map[string]interface{}{
        "name": "changedLabel",
        "languageTag": "en-US",
        "isDefault": true,
    }
}
options := &msgraphsdk.TermRequestBuilderPatchOptions{
    Body: requestBody,
}
setId := "set-id"
termId := "term-id"
graphClient.TermStore().SetsById(&setId).TermsById(&termId).Patch(options)


```