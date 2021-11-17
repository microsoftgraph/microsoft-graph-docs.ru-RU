---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 00ceb0d3f281b2084456863fc250483b1ab1a5f1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = Convert.FromBase64String("base64bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
};

await graphClient.Me.Events["{event-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```