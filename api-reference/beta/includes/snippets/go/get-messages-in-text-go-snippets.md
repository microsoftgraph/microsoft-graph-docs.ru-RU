---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c8fb684489fd6ea59ef87cbed9b6e7293ba1468
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340281"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,uniqueBody",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.MessagesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Me().Messages().GetWithRequestConfigurationAndResponseHandler(options, nil)


```