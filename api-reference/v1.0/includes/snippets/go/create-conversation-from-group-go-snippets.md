---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 25b10daa7b53c3782015a0eb6dbdbf52150925ab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993144"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConversation()
topic := "Take your wellness days and rest"
requestBody.SetTopic(&topic)
requestBody.SetThreads( []ConversationThread {
    msgraphsdk.NewConversationThread(),
    SetAdditionalData(map[string]interface{}{
        "posts":  []Object {
        }
    }
}
options := &msgraphsdk.ConversationsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Conversations().Post(options)


```