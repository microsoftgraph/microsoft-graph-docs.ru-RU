---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dd8433c55d89887bbd25a801a4f89e599cd6046c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceManagementDetails = await graphClient.TenantRelationships.DelegatedAdminCustomers["{delegatedAdminCustomer-id}"].ServiceManagementDetails
    .Request()
    .GetAsync();

```