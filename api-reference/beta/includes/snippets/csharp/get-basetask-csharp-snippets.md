---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a1796a735cb423568f9b67fd004d80565cd55e40
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTask = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"]
    .Request()
    .GetAsync();

```