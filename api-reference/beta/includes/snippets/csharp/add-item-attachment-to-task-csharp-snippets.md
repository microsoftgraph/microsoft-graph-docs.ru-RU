---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3a14cb5c0c02da76839f9efd60d59aea94d26bd41247ea6f1fa6d3f81c9fcbcd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57369874"
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