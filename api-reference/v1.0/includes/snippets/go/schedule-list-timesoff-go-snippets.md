---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d1553db35203670d39e4c77e9a69e2ec7f47c9c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TimesOffRequestBuilderGetQueryParameters{
    Filter: "sharedTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20sharedTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z%20and%20draftTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20draftTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z",
}
options := &msgraphsdk.TimesOffRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOff().GetWithRequestConfigurationAndResponseHandler(options, nil)


```