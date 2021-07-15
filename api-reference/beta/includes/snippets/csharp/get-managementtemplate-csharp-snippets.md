---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d94f2f41ba9fa3e90eb24a9c8be6865517dc3e6e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementTemplate = await graphClient.TenantRelationships.ManagedTenants.ManagementTemplates["{managedTenants.managementTemplate-id}"]
    .Request()
    .GetAsync();

```