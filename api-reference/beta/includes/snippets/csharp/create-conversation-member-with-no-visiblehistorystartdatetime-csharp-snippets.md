---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0477386d5b0c1393ac3ce10b1b4335a6d3627c9f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"}
    }
};

await graphClient.Chats["{chat-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```