---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fb0a0e5d0170112739c30ea8e3ca701683b03653
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSetQuery = new Microsoft.Graph.Ediscovery.ReviewSetQuery
{
    DisplayName = "My Query 1",
    Query = "(subject:\"Quarterly Financials\")"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"].Queries
    .Request()
    .AddAsync(reviewSetQuery);

```