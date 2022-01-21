---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c7648a4414847ba667590c10a1916ff3d8d6ea3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62138288"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
customPrompt := msgraphsdk.NewPrompt()
requestBody.SetCustomPrompt(customPrompt)
customPrompt.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.mediaPrompt",
}
clientContext := "d45324c1-fcb5-430a-902c-f20af696537c"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.StartHoldMusicRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
participantId := "participant-id"
result, err := graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).StartHoldMusic().Post(options)


```