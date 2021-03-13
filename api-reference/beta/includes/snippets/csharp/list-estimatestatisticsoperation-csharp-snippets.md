---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b997660f60fc7c251bdcceacc22b306653e083fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772634"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var estimateStatisticsOperation = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].LastEstimateStatisticsOperation
    .Request()
    .GetAsync();

```