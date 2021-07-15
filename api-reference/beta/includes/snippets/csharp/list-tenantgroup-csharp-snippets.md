---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 97089dcfe8abac4115d270350f2a17913b117a37
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440577"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantGroups = await graphClient.TenantRelationships.ManagedTenants.TenantGroups
    .Request()
    .GetAsync();

```