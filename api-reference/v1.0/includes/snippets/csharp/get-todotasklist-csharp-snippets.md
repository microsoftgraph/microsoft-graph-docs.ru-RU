---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3fff492319c44280acce3d579630d9d2213d3bf6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Me.Todo.Lists
    .Request()
    .GetAsync();

```