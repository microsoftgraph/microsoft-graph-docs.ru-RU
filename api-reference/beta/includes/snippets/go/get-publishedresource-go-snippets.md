---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: edf80847a31ef7271dae6e790aa6e24c8d7f8161
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343110"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PublishedResourceRequestBuilderGetQueryParameters{
    Expand: "agentGroups",
}
options := &msgraphsdk.PublishedResourceRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
publishedResourceId := "publishedResource-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResourcesById(&publishedResourceId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```