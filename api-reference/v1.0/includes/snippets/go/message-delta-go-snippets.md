---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e3528e84124a8a73167e6301cad738eb0efce08
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342323"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "odata.maxpagesize=2"
}
options := &msgraphsdk.DeltaRequestBuilderGetRequestConfiguration{
    Headers: headers,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Messages().Delta()(mailFolder-id).GetWithRequestConfigurationAndResponseHandler(options, nil)


```