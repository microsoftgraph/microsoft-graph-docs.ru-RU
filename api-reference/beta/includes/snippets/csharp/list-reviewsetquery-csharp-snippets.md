---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ff1be8560a767d180e9f95d3edad9f829a15662
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queries = await graphClient.Compliance.Ediscovery.Cases["2eef613a-ca2d-42f4-89fe-84d5198ddedf"].ReviewSets["b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8"].Queries
    .Request()
    .GetAsync();

```