---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2b00579d0a974b9cb22724b61c42218c10eb7be
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63416523"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInferenceClassificationOverride()
classifyAs := "focused"
requestBody.SetClassifyAs(&classifyAs)
options := &msgraphsdk.InferenceClassificationOverrideRequestBuilderPatchOptions{
    Body: requestBody,
}
inferenceClassificationOverrideId := "inferenceClassificationOverride-id"
result, err := graphClient.Me().InferenceClassification().OverridesById(&inferenceClassificationOverrideId).Patch(options)


```