---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 85de9f94cdf2a001367bda8fadf24e5173b26cb6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123573"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistration = new ExternalMeetingRegistration
{
    AllowedRegistrant = MeetingAudience.Everyone
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration
    .Request()
    .AddAsync(meetingRegistration);

```