---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dba00f48afa6327388acbb821a416fd92b0e8ead
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = await graphClient.Users["{user-id}"].Calendar.CalendarPermissions["{calendarPermission-id}"]
    .Request()
    .GetAsync();

```