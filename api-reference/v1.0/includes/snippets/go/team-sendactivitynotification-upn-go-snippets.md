---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b47edfea332ae9a0e6d921900cdba4aa258b95ce
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342927"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
topic.SetValue(&value)
activityType := "reservationUpdated"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "You have moved up the queue"
previewText.SetContent(&content)
recipient := msgraphsdk.NewTeamworkNotificationRecipient()
requestBody.SetRecipient(recipient)
recipient.SetAdditionalData(map[string]interface{}{
    "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
    "userId": "jacob@contoso.com",
}
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
    SetAdditionalData(map[string]interface{}{
        "name": "reservationId",
        "value": "TREEE433",
    }
    msgraphsdk.NewKeyValuePair(),
    SetAdditionalData(map[string]interface{}{
        "name": "currentSlot",
        "value": "23",
    }
}
teamId := "team-id"
graphClient.TeamsById(&teamId).SendActivityNotification(team-id).Post(requestBody)


```