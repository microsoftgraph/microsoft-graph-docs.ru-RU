---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c2eaf5dcf6966aac09dc18e739ef02cb0520b15d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340090"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ListRequestBuilderGetQueryParameters{
    Select: "id,name,lastModifiedDateTime",
    Expand: "columns(select=name,description),items)",
}
options := &msgraphsdk.ListRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```