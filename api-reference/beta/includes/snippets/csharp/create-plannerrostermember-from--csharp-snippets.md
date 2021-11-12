---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dd654f3c7d2900a8ff9478d90e98c6cbf88d9c97c13fd17c665cd38c69ed3c30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRosterMember = new PlannerRosterMember
{
    UserId = "String"
};

await graphClient.Planner.Rosters["{plannerRoster-id}"].Members
    .Request()
    .AddAsync(plannerRosterMember);

```