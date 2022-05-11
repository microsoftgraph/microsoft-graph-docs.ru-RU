---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ef874e8826dc56601d6fbd544d4d18df46907d8f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341464"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNoncustodialDataSource()
applyHoldToSource := false
requestBody.SetApplyHoldToSource(&applyHoldToSource)
dataSource := msgraphsdk.NewDataSource()
requestBody.SetDataSource(dataSource)
dataSource.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.ediscovery.siteSource",
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).NoncustodialDataSources().Post(requestBody)


```