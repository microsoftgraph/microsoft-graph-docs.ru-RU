---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 511d058b3760009e8e9cff8a341d05ffa4814f13
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695281"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
pinnedChatMessageInfoId := "pinnedChatMessageInfo-id"
graphClient.ChatsById(&chatId).PinnedMessagesById(&pinnedChatMessageInfoId).Delete()


```