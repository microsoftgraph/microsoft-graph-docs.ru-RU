---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 291feadee92912cb1fe89f5deddb72e45616f793
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrantBase = new ExternalMeetingRegistrant
{
    Id = "9d96988d-a66a-46ce-aad7-0b245615b297"
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.Registrants
    .Request()
    .AddAsync(meetingRegistrantBase);

```