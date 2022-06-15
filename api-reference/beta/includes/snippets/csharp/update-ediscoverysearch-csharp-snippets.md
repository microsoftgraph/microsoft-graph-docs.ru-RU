---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 998ad0fdfcc03fad1c1bbb479bf3412b302c2557
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoverySearch = new Microsoft.Graph.Security.EdiscoverySearch
{
    DisplayName = "Teams search"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"]
    .Request()
    .UpdateAsync(ediscoverySearch);

```