---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46e3b9aea2e3c93bee828424946ff5b71aacd7bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802425"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "topic-value",
    Posts = new ConversationThreadPostsCollectionPage()
    {
        new Post
        {
            Body = new ItemBody
            {
                ContentType = BodyType.Html,
                Content = "this is body content"
            }
        }
    }
};

await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"].Threads
    .Request()
    .AddAsync(conversationThread);

```