---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f521a22dda77ecb3aa169e2dff177c2e4c97da6c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "name-value"
};

await graphClient.Me.CalendarGroups["{id}"]
    .Request()
    .UpdateAsync(calendarGroup);

```