---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d3094d8f23eb96ce9f00dddbc4302cb7142ea3e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488879"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    AdditionalInformation = "additionalInformation-after-update",
    Confidence = 42,
    Description = "description-after-update"
};

await graphClient.Security.TiIndicators["{id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(tiIndicator);

```