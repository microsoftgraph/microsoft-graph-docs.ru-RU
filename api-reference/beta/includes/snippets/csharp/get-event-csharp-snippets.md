---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 36ab3146494651a8cf43cab0cab592ab3aff3786
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["{event-id}"]
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .Select("subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees")
    .GetAsync();

```