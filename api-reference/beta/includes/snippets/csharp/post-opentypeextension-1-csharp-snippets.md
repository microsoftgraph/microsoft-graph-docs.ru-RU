---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44643064b53829741042a604fb082ab2e9575681
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Annual review",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "You should be proud!"
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "rufus@contoso.com"
            }
        }
    },
    Extensions = new List<Extension>()
    {
        new Extension
        {
            ExtensionName = "Com.Contoso.Referral",
            CompanyName = "Wingtip Toys",
            ExpirationDate = "2015-12-30T11:00:00Z",
            DealValue = 10000
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```