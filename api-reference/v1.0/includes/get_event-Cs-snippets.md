---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 827baec86d11ce2ee3af4671531c2c27444ab467
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkAGIAAAoZDOFAAA="]
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .Select( e => new {
             e.Subject,
             e.Body,
             e.BodyPreview,
             e.Organizer,
             e.Attendees,
             e.Start,
             e.End,
             e.Location 
             })
    .GetAsync();

```