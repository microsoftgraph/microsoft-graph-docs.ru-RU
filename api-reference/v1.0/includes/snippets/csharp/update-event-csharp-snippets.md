---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 568047a4d12ad15e821847c885c9440aa9b68668
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228375"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    OriginalStartTimeZone = "originalStartTimeZone-value",
    OriginalEndTimeZone = "originalEndTimeZone-value",
    ResponseStatus = new ResponseStatus
    {
        Response = ResponseType.None,
        Time = DateTimeOffset.Parse("datetime-value")
    },
    Recurrence = null,
    ReminderMinutesBeforeStart = 99,
    IsOnlineMeeting = true,
    OnlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness,
    IsReminderOn = true,
    HideAttendees = false,
    Categories = new List<String>()
    {
        "Red category"
    }
};

await graphClient.Me.Events["{event-id}"]
    .Request()
    .UpdateAsync(@event);

```