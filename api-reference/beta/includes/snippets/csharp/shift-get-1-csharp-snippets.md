---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bdf2a8bd05652d7fac860563c75aa86e594db12b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = await graphClient.Teams["{team-id}"].Schedule.Shifts["{shift-id}"]
    .Request()
    .GetAsync();

```