---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 723a469434b52e8d7b724b102d2b1f594ae4bc7f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094699"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryReviewSetQuery = new Microsoft.Graph.Security.EdiscoveryReviewSetQuery
{
    DisplayName = "My Query 1",
    ContentQuery = "(Author=\"edison\")"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"].Queries
    .Request()
    .AddAsync(ediscoveryReviewSetQuery);

```