---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c6a894feb2e5ac1393176739c7537ebe4cff6c2b1ef749b042924065c22c4397
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57319140"
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