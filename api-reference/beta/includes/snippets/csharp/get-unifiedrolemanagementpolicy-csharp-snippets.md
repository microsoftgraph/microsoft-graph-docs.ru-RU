---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 04d2e8c6c804b38cca0f78d44520c0b0fb91b154
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicy = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"]
    .Request()
    .GetAsync();

```