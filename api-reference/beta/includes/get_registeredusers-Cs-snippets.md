---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0dc71b6cb192b5faef6296aed191ea9590a3cab5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446839"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredUsers = await graphClient.Devices["{id}"].RegisteredUsers
    .Request()
    .GetAsync();

```