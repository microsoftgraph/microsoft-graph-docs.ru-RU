---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2bfc43209e7a692bb82545ea9a1eb581465ca470
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = new Microsoft.Graph.Ediscovery.Case
{
    DisplayName = "My Case 1"
};

await graphClient.Compliance.Ediscovery.Cases
    .Request()
    .AddAsync(@case);

```