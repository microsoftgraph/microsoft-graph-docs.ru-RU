---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 671f9387162498ed233ab8c5b1821f4817076928
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806559"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = new CalendarPermission();
calendarPermission.role = CalendarRoleType.WRITE;

graphClient.users("{id}").calendar().calendarPermissions("RGVmYXVsdA==")
    .buildRequest()
    .patch(calendarPermission);

```