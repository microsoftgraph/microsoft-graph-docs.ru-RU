---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ab98096d9b12e4c4087ac038dbf51750f7c7c5a8
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996235"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    EmailAddress = new EmailAddress
    {
        Name = "Samantha Booth",
        Address = "samanthab@adatum.onmicrosoft.com"
    },
    IsInsideOrganization = true,
    IsRemovable = true,
    Role = CalendarRoleType.Read
};

await graphClient.Me.Calendar.CalendarPermissions
    .Request()
    .AddAsync(calendarPermission);

```