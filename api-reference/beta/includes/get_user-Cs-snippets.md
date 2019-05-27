---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: df033299fdf749885fa325181e5184f66d0d740a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Me
    .Request()
    .GetAsync();

```