---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5c67a493abcb696adacef2fdf4a7c397f444fe27
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795597"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedulingGroup = await graphClient.Teams["{team-id}"].Schedule.SchedulingGroups["{schedulingGroup-id}"]
    .Request()
    .GetAsync();

```