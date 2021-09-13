---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 543256eefeab3955fc35620bd2acd7528c116d36815ec76df3fe30c1cbe98912
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57311789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedulingGroups = await graphClient.Teams["{team-id}"].Schedule.SchedulingGroups
    .Request()
    .GetAsync();

```