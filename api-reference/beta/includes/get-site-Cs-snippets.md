---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5440ed31d45771f32dadcd29054baeeacf3ad359
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var site = await graphClient.Sites["{site-id}"]
    .Request()
    .GetAsync();

```