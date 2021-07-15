---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a8b82c74ee7b61b523d720b0c445c539e93af48
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantCustomizedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation["{managedTenants.tenantCustomizedInformation-id}"]
    .Request()
    .GetAsync();

```