---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ad7308f14cd4bdc8624d1769a6c1c4439464b6ed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = await graphClient.RoleManagement.DeviceManagement.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .GetAsync();

```