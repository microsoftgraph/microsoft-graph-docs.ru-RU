---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d1fc44c7e4d8559977c556e04f945204afd32c903f9059df02e1cfa5c9c64e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57253900"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTag = new Microsoft.Graph.ManagedTenants.TenantTag
{
    DisplayName = "Onboarding",
    Description = "Tenants that we are currently onboarding"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .Request()
    .UpdateAsync(tenantTag);

```