---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c7471b1a898fa09250f7fc270a3e5d7d9664fb5
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844302"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var apiConnectors = await graphClient.Identity.ApiConnectors
    .Request()
    .GetAsync();

```