---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 12907886afb51af0629205219285e547e1c45c1a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminCustomer = await graphClient.TenantRelationships.DelegatedAdminCustomers["{delegatedAdminCustomer-id}"]
    .Request()
    .GetAsync();

```