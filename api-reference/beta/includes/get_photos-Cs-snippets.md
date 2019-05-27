---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff2849f23da9b870be81a80f9db9c1428283caed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var photos = await graphClient.Groups["{id}"].Photos
    .Request()
    .GetAsync();

```