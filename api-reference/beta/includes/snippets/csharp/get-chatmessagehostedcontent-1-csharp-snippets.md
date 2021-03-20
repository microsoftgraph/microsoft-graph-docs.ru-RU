---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b481c42846b6460de1ffceebdc35ae7dcff2a96
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947772"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessageHostedContent = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents["{chatMessageHostedContent-id}"]
    .Request()
    .GetAsync();

```