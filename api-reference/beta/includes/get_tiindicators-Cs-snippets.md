---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ffe7448a8c5cd1e8294f5a0cb77349837bb7e04
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445331"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicators = await graphClient.Security.TiIndicators
    .Request()
    .GetAsync();

```