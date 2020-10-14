---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5b55ac6f66ca1e20d518d4403a59e7d9aeb26c8f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = new Microsoft.Graph.TermStore.Store
{
    DefaultLanguageTag = "en-US"
};

await graphClient.TermStore
    .Request()
    .UpdateAsync(store);

```