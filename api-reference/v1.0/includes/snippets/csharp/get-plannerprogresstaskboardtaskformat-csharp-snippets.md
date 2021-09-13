---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 78c1f97dcf6cec64cfb254e77720dc6a2ecbb42f2681864050bdb20bbee66671
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57432352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = await graphClient.Planner.Tasks["{plannerTask-id}"].ProgressTaskBoardFormat
    .Request()
    .GetAsync();

```