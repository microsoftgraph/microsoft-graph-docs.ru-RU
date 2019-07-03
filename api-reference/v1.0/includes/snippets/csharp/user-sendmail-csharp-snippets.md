---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 700bce7b4a331c6072582ddd9a8ca3c479decbf4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35473043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Meet for lunch?",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "The new cafeteria is open."
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "fannyd@contoso.onmicrosoft.com"
            }
        }
    },
    CcRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "danas@contoso.onmicrosoft.com"
            }
        }
    }
};

var saveToSentItems = false;

await graphClient.Me
    .SendMail(message,saveToSentItems)
    .Request()
    .PostAsync();

```