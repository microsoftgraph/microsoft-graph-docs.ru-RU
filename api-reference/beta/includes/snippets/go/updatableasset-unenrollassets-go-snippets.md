---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ac9c91d7b14e957668bd4445143fe86ac24190d8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085944"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
updateCategory := "String"
requestBody.SetUpdateCategory(&updateCategory)
requestBody.SetAssets( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
        "id": "String (identifier)",
    }
}
options := &msgraphsdk.UnenrollAssetsRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Admin().Windows().Updates().UpdatableAssets().UnenrollAssets().Post(options)


```