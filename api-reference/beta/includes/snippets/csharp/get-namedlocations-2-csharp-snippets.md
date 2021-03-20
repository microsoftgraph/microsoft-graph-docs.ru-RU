---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 258c6a164a1dacf8053e499c663f189874ec2158
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .Filter("isof('microsoft.graph.ipNamedLocation')")
    .GetAsync();

```