---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 12065c13a0c7e6ba103025ff3cd6cc28bb8c43fc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = await graphClient.Planner.Plans["{plan-id}"]
    .Request()
    .GetAsync();

```