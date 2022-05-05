---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ffa06c1317d5b364bdee2436d9937ed3487d670
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleInstance = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleInstances["{unifiedRoleAssignmentScheduleInstance-id}"]
    .Request()
    .GetAsync();

```