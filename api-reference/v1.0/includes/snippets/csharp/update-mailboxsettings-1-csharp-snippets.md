---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9102d176b144039ea6bb4dfea2960fe833da6e6e
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684961"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailboxSettings = new MailboxSettings
{
    AutomaticRepliesSetting = new AutomaticRepliesSetting
    {
        Status = AutomaticRepliesStatus.Scheduled,
        ScheduledStartDateTime = new DateTimeTimeZone
        {
            DateTime = "2016-03-20T18:00:00",
            TimeZone = "UTC"
        },
        ScheduledEndDateTime = new DateTimeTimeZone
        {
            DateTime = "2016-03-28T18:00:00",
            TimeZone = "UTC"
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.context", "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings"}
    }
};

var me = new User();
me.MailboxSettings = mailboxSettings;

await graphClient.Me
    .Request()
    .UpdateAsync(me);

```