---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 16327e67e312ebcb5e1e86dfa4b929e336520927
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993921"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPublishedResource()
displayName := "Demo provisioning (updated)"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.PublishedResourceRequestBuilderPatchOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
publishedResourceId := "publishedResource-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResourcesById(&publishedResourceId).Patch(options)


```