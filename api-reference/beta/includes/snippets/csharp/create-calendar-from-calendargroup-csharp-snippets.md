---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a2c22475d853b3015ea362299385d9cfd71c90cb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808683"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Marketing calendar"
};

await graphClient.Me.CalendarGroups["{calendarGroup-id}"].Calendars
    .Request()
    .AddAsync(calendar);

```