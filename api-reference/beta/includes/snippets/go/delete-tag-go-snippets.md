---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a09c836720681791a948be82d6341e2297d272c4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343001"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TagRequestBuilderDeleteQueryParameters{
    Forcedelete: true,
}
options := &msgraphsdk.TagRequestBuilderDeleteRequestConfiguration{
    QueryParameters: requestParameters,
}
caseId := "case-id"
tagId := "tag-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).DeleteWithRequestConfigurationAndResponseHandler(options, nil)


```