---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 71a76a997f548cfc400dd0a1b6ef6916422e9c52f71944cd9c8d5b33c54a8dd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57193409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenant = await graphClient.TenantRelationships.ManagedTenants.Tenants["{managedTenants.tenant-id}"]
    .Request()
    .GetAsync();

```