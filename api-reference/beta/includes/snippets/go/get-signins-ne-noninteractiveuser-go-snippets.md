---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e505b84bff22219a3cb30d82360733a4e9853110
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342229"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SignInsRequestBuilderGetQueryParameters{
    Filter: "(signInEventTypes/any(t:%20t%20ne%20'interactiveUser'))",
    OrderBy: "createdDateTime%20DESC",
    Top: 10,
}
options := &msgraphsdk.SignInsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.AuditLogs().SignIns().GetWithRequestConfigurationAndResponseHandler(options, nil)


```