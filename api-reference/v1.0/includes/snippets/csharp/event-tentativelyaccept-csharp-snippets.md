---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 012afc22312bb24279b629aba9c673b38402ac262176ded371e52b76993c9161
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57201105"
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

await graphClient.Me.Events["{event-id}"]
    .TentativelyAccept(comment,sendResponse,proposedNewTime)
    .Request()
    .PostAsync();

```