---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2782e37b063f8aba8d555ec2336cbbf6232221cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032416"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConversationThread()
requestBody.SetAdditionalData(map[string]interface{}{
    "originalStartTimeZone": "originalStartTimeZone-value",
    "originalEndTimeZone": "originalEndTimeZone-value",
    "uid": "iCalUId-value",
    "reminderMinutesBeforeStart": ,
    "isReminderOn": true,
}
options := &msgraphsdk.ConversationThreadRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Patch(options)


```