---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 38c913acebbd2eeaf78f5306457c5b9e53d73c13
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086847"
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
siteId := "site-id"
setId := "set-id"
termId := "term-id"
graphClient.SitesById(&siteId).TermStore().SetsById(&setId).TermsById(&termId).Patch(options)


```