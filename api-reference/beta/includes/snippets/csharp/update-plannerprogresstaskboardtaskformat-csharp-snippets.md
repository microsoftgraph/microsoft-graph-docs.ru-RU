---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3228625ad246f291ef09bc9e81799122783a43b9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat
{
    OrderHint = "A6673H Ejkl!"
};

await graphClient.Planner.Tasks["{plannerTask-id}"].ProgressTaskBoardFormat
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerProgressTaskBoardTaskFormat);

```