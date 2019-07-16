---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99f7923097a4726d9343b3c1939cf88f04c1ff64
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Groups.Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select( e => new {
             e.DisplayName,
             e.Description,
             e.MailNickname 
             })
    .GetAsync();

```