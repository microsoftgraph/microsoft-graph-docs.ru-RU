---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 551846f3ca9b23eb1e54873960255a0e99ae5039
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRoster = await graphClient.Planner.Rosters["{plannerRoster-id}"]
    .Request()
    .GetAsync();

```