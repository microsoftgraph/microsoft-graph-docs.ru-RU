---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b24fa804f2eb5ee82ac346a662d20bfbdaa1f5c3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343525"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ThreatAssessmentRequestRequestBuilderGetQueryParameters{
    Expand: "results",
}
options := &msgraphsdk.ThreatAssessmentRequestRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
threatAssessmentRequestId := "threatAssessmentRequest-id"
result, err := graphClient.InformationProtection().ThreatAssessmentRequestsById(&threatAssessmentRequestId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```