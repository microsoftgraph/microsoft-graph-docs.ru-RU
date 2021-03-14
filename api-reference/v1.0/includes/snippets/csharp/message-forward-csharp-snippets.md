---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: db9781a636bc12476e524c0b73b92eacf8cbc339
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var toRecipients = new List<Recipient>()
{
    new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    }
};

await graphClient.Me.Messages["{message-id}"]
    .Forward(toRecipients,null,comment)
    .Request()
    .PostAsync();

```