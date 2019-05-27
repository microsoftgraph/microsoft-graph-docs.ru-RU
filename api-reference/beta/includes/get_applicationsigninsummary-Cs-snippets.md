---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e9143c487bfa18897525ea7139e65df44ae584d4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAzureADApplicationSignInSummary = await graphClient.Reports.GetAzureADApplicationSignInSummary('D7')
    .Request()
    .GetAsync();

```