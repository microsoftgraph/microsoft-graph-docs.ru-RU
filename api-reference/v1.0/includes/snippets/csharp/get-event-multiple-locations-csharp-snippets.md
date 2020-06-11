---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d551dc6a050682848ad45de2a00741163488a44
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkADAGAADDdm4NAAA="]
    .Request()
    .Select("subject,body,bodyPreview,organizer,attendees,start,end,location,locations")
    .GetAsync();

```