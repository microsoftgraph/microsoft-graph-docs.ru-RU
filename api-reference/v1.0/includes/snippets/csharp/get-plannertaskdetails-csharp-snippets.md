---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 734de2abb51ea3673536da813cf5d64ec752b382
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["{plannerTask-id}"].Details
    .Request()
    .GetAsync();

```