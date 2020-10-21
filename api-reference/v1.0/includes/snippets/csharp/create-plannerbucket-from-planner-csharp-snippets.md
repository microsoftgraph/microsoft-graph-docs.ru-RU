---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c1f49cfe4fc6c0f3bb63b7e7cbcaeb078940d05b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620353"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = new PlannerBucket
{
    Name = "Advertising",
    PlanId = "xqQg5FS2LkCp935s-FIFm2QAFkHM",
    OrderHint = " !"
};

await graphClient.Planner.Buckets
    .Request()
    .AddAsync(plannerBucket);

```