---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9297e516369b5ec6cd14dbdbfbad01ea7803f17a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = new OutlookTask
{
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-05-06T16:00:00",
        TimeZone = "Eastern Standard Time"
    }
};

await graphClient.Me.Outlook.Tasks["AAMkADA1MTHgwAAA="]
    .Request()
    .Header("Prefer","outlook.timezone=\"Eastern Standard Time\"")
    .UpdateAsync(outlookTask);

```