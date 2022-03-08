---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8006bcc3917b19c64fb9edaeb0bd6b9988ef13fb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acronym = new Microsoft.Graph.Search.Acronym
{
    Description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
};

await graphClient.Search.Acronyms["{search.acronym-id}"]
    .Request()
    .UpdateAsync(acronym);

```