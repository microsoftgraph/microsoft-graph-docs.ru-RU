---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a9b9079cceb3a86ce176464539173a2c77925693
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTaskList = new BaseTaskList
{
    DisplayName = "Shopping list"
};

await graphClient.Me.Tasks.Lists
    .Request()
    .AddAsync(baseTaskList);

```