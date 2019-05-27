---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 691b4ae1633ce91fa60e274e9743edd52ef72755
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469323"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<String>()
{
    "id-value1",
    "id-value2"
};

await graphClient.Security.TiIndicators
    .DeleteTiIndicators(value)
    .Request()
    .PostAsync();

```