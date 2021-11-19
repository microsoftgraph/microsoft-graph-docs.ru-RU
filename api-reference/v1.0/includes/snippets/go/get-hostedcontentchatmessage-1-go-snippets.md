---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d63f8d0de8f5eb989cb36e9ac6007ac5965d7045
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084129"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
chatMessageHostedContentId := "chatMessageHostedContent-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContentsById(&chatMessageHostedContentId).Get(options)


```