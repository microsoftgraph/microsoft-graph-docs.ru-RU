---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3eb0d9f14b16129badcaadbab409cf448db0f469
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ListItemRequestBuilderGetQueryParameters{
    Expand: "fields",
}
options := &msgraphsdk.ListItemRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```