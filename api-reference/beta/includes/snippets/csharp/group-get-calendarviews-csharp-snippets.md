---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 82af2848fc88a107ea26ee7290949240dbb1e870
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803820"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2017-01-01T19:00:00-08:00"),
    new QueryOption("endDateTime", "2017-10-01T19:00:00.00-08:00")
};

var calendarView = await graphClient.Groups["{group-id}"].CalendarView
    .Request( queryOptions )
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .GetAsync();

```