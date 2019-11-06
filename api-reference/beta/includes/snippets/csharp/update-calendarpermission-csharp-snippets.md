---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9f221ae830abe79338d74ef5bf4fdade0ad24532
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    EmailAddress = new EmailAddress
    {
        Name = "My Organization"
    },
    IsRemovable = true,
    IsInsideOrganization = true,
    Role = CalendarRoleType.Write,
    AllowedRoles = new List<CalendarRoleType>()
    {
        CalendarRoleType.None,
        CalendarRoleType.FreeBusyRead,
        CalendarRoleType.LimitedRead,
        CalendarRoleType.Read,
        CalendarRoleType.Write
    },
    Id = "RGVmYXVsdA=="
};

await graphClient.Users["{id}"].Calendar.CalendarPermissions["{id}"]
    .Request()
    .UpdateAsync(calendarPermission);

```