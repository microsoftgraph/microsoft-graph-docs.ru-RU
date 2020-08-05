---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ef00c46f29cdd05a3480adba33ac5b587457d8bf
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566608"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganization = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{id}"]
    .Request()
    .GetAsync();

```