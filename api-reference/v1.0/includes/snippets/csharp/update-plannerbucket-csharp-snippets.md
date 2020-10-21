---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 93cb69f7e46d31b89baf90c42f12fb299edf85b0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = new PlannerBucket
{
    Name = "Development"
};

await graphClient.Planner.Buckets["{bucket-id}"]
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerBucket);

```