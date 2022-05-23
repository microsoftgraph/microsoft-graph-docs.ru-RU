---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0543b03580531f081763a285d71d686505a86605
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantUsage = await graphClient.TenantRelationships.ManagedTenants.TenantUsage
    .Request()
    .GetAsync();

```