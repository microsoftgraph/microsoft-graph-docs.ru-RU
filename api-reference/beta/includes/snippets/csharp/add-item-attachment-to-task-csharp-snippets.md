---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 798c5c136adc1d4ffa5462da32c1e767c287c81a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796747"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new ItemAttachment
{
    Name = "Holiday event",
    Item = new Event
    {
        Subject = "Discuss gifts for children",
        Body = new ItemBody
        {
            ContentType = BodyType.Html,
            Content = "Let's look for funding!"
        },
        Start = new DateTimeTimeZone
        {
            DateTime = "2020-01-12T18:00:00",
            TimeZone = "Pacific Standard Time"
        },
        End = new DateTimeTimeZone
        {
            DateTime = "2020-01-12T19:00:00",
            TimeZone = "Pacific Standard Time"
        }
    }
};

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```