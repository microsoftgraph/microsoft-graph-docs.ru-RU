---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a15441e7e907e29762b179a8ea20c9eff324a718df40b09a3a98af8c7189fda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57320054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = new PlannerAssignedToTaskBoardTaskFormat
{
    OrderHintsByAssignee = new PlannerOrderHintsByAssignee
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"aaa27244-1db4-476a-a5cb-004607466324", "8566473P 957764Jk!"}
        }
    }
};

await graphClient.Planner.Tasks["{plannerTask-id}"].AssignedToTaskBoardFormat
    .Request()
    .Header("Prefer","return=representation")
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerAssignedToTaskBoardTaskFormat);

```