---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 352f9111d93db35f6a62b5166b9ebfc1a3fc1012
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340143"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SourceCollectionRequestBuilderGetQueryParameters{
    Expand: "addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation",
}
options := &msgraphsdk.SourceCollectionRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```