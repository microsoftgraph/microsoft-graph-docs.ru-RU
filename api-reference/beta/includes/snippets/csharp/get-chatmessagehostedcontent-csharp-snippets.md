---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0a4c1c028226702ee40c02f3cfeb14331dfe9336
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents["{chatMessageHostedContent-id}"].Content
    .Request()
    .GetAsync();

```