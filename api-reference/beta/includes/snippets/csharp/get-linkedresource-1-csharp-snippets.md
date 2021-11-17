---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 58d6bd8708184046a03655963b0e2f48cedfbcf5afe1dd1ff70d1cc46e547410
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57263818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResource = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].LinkedResources["{linkedResource-id}"]
    .Request()
    .GetAsync();

```