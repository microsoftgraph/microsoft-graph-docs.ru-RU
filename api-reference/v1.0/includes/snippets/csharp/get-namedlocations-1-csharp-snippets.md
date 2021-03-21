---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 26ca39d9e00384640269fcf6c447ead4c1c13a2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .GetAsync();

```