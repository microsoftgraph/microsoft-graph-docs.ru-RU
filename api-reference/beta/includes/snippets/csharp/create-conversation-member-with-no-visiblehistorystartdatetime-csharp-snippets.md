---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 091fc5b6ecde02f7c558a4836ff329215dc118e4f5dfad3f225fdcf8edf8473e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
        "owner"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"}
    }
};

await graphClient.Chats["{chat-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```