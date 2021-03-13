---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 946e958e05a1101cee2141c96fdcec333a6d4be9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808083"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "name-value",
    ContentType = "contentType-value",
    IsInline = false,
    ContentLocation = "contentLocation-value",
    ContentBytes = Encoding.ASCII.GetBytes("contentBytes-value")
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```