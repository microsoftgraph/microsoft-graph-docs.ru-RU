---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 65850c3202f6a6de6407c2594efef58bdd55ac74
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = new Conversation
{
    Topic = "New locations for this quarter",
    Threads = new ConversationThreadsCollectionPage()
    {
        new ConversationThread
        {
            Posts = new ConversationThreadPostsCollectionPage()
            {
                new Post
                {
                    Body = new ItemBody
                    {
                        ContentType = BodyType.Html,
                        Content = "What do we know so far?"
                    },
                    NewParticipants = new List<Recipient>()
                    {
                        new Recipient
                        {
                            EmailAddress = new EmailAddress
                            {
                                Name = "Adele Vance",
                                Address = "AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    }
                }
            }
        }
    }
};

await graphClient.Groups["{group-id}"].Conversations
    .Request()
    .AddAsync(conversation);

```