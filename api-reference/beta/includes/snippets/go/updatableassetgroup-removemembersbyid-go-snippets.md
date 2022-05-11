---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6148819e65344c3285386ce50b42c25eda24c640
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341130"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetIds( []String {
    "String",
    "String",
    "String",
}
memberEntityType := "#microsoft.graph.windowsUpdates.azureADDevice"
requestBody.SetMemberEntityType(&memberEntityType)
updatableAssetId := "updatableAsset-id"
graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).RemoveMembersById(updatableAsset-id).Post(requestBody)


```