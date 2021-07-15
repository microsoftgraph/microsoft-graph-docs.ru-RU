---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 57448d1ca13ed6bc184489bb924dcb737e2c691e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantIds = new List<String>()
{
    "String"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .AssignTag(tenantIds)
    .Request()
    .PostAsync();

```