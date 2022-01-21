---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e9893365be83d682c73b03f0e1891e2c4bc9b2c2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62138297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantCustomizedInformation = new Microsoft.Graph.ManagedTenants.TenantCustomizedInformation
{
    TenantId = "String",
    Contacts = new List<Microsoft.Graph.ManagedTenants.TenantContactInformation>()
    {
        new TenantContactInformation
        {
            Name = "String",
            Title = "String",
            Email = "String",
            Phone = "String",
            Notes = "String"
        }
    },
    Website = "String"
};

await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation["{managedTenants.tenantCustomizedInformation-id}"]
    .Request()
    .UpdateAsync(tenantCustomizedInformation);

```