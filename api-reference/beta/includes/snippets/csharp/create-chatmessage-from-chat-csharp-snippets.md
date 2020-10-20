---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 324ff328216d6f30ac5e54a6156fbba102e6c1b3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618063"
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

await graphClient.Teams["{id}"].Channels["{id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```