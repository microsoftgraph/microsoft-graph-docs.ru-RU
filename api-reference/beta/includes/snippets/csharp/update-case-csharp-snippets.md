---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 944ec36085173c343fe0659c0a5676687598004b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = new Microsoft.Graph.Ediscovery.Case
{
    DisplayName = "My Case 1 - Renamed",
    Description = "Updated description",
    ExternalId = "Updated externalId"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Request()
    .UpdateAsync(@case);

```