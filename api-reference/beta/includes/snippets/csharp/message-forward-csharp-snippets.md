---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 48e5d70d341917ea7a7059e6b62037400f60198e1adcd13c7b29f1fef7942374
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57269940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsDeliveryReceiptRequested = true,
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "danas@contoso.onmicrosoft.com",
                Name = "Dana Swope"
            }
        }
    }
};

var comment = "Dana, just want to make sure you get this.";

await graphClient.Me.Messages["{message-id}"]
    .Forward(null,message,comment)
    .Request()
    .PostAsync();

```