---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ddad74c63e7da36931e182ff731b2adbe931c67dd081d34878905c80cd857119
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = new Chat
{
    Topic = "Group chat title update"
};

await graphClient.Chats["{chat-id}"]
    .Request()
    .UpdateAsync(chat);

```