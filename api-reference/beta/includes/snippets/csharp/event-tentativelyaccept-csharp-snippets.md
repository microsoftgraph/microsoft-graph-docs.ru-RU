---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc5e4cc41baeb705a1fb01354ce78f1d380c33cc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "I may not be able to make this week. How about next week?";

var sendResponse = true;

var proposedNewTime = new TimeSlot
{
    Start = new DateTimeTimeZone
    {
        DateTime = "2019-12-02T18:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2019-12-02T19:00:00",
        TimeZone = "Pacific Standard Time"
    }
};

await graphClient.Me.Events["{id}"]
    .TentativelyAccept(proposedNewTime,sendResponse,comment)
    .Request()
    .PostAsync();

```