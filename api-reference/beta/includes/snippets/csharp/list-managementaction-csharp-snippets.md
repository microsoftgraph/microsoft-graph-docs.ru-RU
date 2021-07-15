---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09a0591e7e4898bf1be89679abeb1ae087c0bb54
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442500"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActions = await graphClient.TenantRelationships.ManagedTenants.ManagementActions
    .Request()
    .GetAsync();

```