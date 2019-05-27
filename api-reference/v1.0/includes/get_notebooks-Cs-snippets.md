---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b2936b66a608d86810f1ee940254f135684a0b2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebooks = await graphClient.Me.Onenote.Notebooks
    .Request()
    .GetAsync();

```