---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7391f98f04b897b2d736f3f307745d958239bcdf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788180"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = new PlannerPlan
{
    Title = "title-value"
};

await graphClient.Planner.Plans["{plannerPlan-id}"]
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerPlan);

```