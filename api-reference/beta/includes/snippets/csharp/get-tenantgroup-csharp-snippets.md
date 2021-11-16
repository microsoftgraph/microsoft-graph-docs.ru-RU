---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 22f1d15aa4c87e83eefd8b3f075547f5cc571f7ac38ed4b14b5b5c6c5d88d646
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57314320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantGroup = await graphClient.TenantRelationships.ManagedTenants.TenantGroups["{managedTenants.tenantGroup-id}"]
    .Request()
    .GetAsync();

```