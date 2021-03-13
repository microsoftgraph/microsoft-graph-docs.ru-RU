---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d23bd9f4edf628646f5decca24fdc2921290ee7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rosterPlans = await graphClient.Users["{user-id}"].Planner.RosterPlans
    .Request()
    .GetAsync();

```