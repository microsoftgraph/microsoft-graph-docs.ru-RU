---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fed5d5ec5540a64bd86292b656fd2de2b58ce5a2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778232"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    Role = CalendarRoleType.Write
};

await graphClient.Users["{user-id}"].Calendar.CalendarPermissions["{calendarPermission-id}"]
    .Request()
    .UpdateAsync(calendarPermission);

```