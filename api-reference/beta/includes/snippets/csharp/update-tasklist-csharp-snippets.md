---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f85ef8841b96f653b07c374999a9d97f5185f438
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTaskList = new TaskList
{
    DisplayName = "Travel Plan"
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"]
    .Request()
    .UpdateAsync(baseTaskList);

```