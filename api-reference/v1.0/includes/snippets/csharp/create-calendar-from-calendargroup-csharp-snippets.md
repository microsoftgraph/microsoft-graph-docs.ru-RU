---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ae1e7eb7d686cb92b33e229ca076ccc5b52840e0fd84ed9c7b46c1f0420b60b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364007"
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