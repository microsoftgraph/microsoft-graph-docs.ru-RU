---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 60a5276e56cd1fb6bb6e454ce0c4033c4e4c6ed4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025955"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ChatRequestBuilderGetQueryParameters{
    Top: 2,
}
options := &msgraphsdk.ChatRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
chatId := "chat-id"
result, err := graphClient.UsersById(&userId).ChatsById(&chatId).Get(options)


```