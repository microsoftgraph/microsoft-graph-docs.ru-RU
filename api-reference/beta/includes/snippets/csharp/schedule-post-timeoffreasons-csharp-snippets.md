---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f52f87b8be46e03c60c50c7eb40c43cc297b895e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReason = new TimeOffReason
{
    DisplayName = "Vacation",
    IconType = TimeOffReasonIconType.Plane,
    IsActive = true
};

await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons
    .Request()
    .AddAsync(timeOffReason);

```