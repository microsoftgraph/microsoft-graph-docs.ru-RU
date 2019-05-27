---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bac0f098e633c8839f11e356a4eb688e18c6192e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedAdministratorOf = await graphClient.Me.ScopedAdministratorOf
    .Request()
    .GetAsync();

```