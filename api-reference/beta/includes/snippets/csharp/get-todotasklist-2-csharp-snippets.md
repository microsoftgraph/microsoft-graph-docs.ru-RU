---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 601c76843c90a3b522f7df11309a7d11c916dc83b843ec965a62fc8a782813ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57312294"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = await graphClient.Me.Todo.Lists["{todoTaskList-id}"]
    .Request()
    .GetAsync();

```