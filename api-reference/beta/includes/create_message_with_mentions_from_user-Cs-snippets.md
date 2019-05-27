---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 249ce76e9c70303b805ff8da5a3a7b0f9b2345a7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Party planning",
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Name = "Samantha Booth",
                Address = "samanthab@contoso.onmicrosoft.com"
            }
        }
    },
    Mentions = new List<Mention>()
    {
        new Mention
        {
            Mentioned = new EmailAddress
            {
                Name = "Dana Swope",
                Address = "danas@contoso.onmicrosoft.com"
            }
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```