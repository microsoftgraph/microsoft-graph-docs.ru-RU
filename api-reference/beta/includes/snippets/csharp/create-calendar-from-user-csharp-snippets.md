---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0e5669575a61028f928f917d8180b6db08f8a2e1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Volunteer"
};

await graphClient.Me.Calendars
    .Request()
    .AddAsync(calendar);

```