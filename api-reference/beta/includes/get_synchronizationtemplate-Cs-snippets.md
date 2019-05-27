---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 957b0e8db1a6c2094b3b51b04bd043cee6f15d56
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445730"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var templates = await graphClient.ServicePrincipals["{id}"].Synchronization.Templates
    .Request()
    .GetAsync();

```