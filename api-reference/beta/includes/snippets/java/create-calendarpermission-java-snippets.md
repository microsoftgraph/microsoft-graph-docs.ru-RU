---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 69c76723ee51906b06deb440212218a61113994b
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995703"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = new CalendarPermission();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "Samantha Booth";
emailAddress.address = "samanthab@adatum.onmicrosoft.com";
calendarPermission.emailAddress = emailAddress;
calendarPermission.isInsideOrganization = true;
calendarPermission.isRemovable = true;
calendarPermission.role = CalendarRoleType.READ;

graphClient.users("458d4c95-124e-49da-ba9d-1dd0387e682e").calendar().calendarPermissions()
    .buildRequest()
    .post(calendarPermission);

```