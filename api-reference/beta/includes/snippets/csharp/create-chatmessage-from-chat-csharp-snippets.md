---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1c1eb4f2f26b7eb1ffccc797d8f37e94c1eb8939
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        Content = "Hello world"
    }
};

await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```