---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b9cc15108294a20cc2f267ff2aa032f372e987e4
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514310"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleInstances
    .FilterByCurrentUser(RoleAssignmentScheduleInstanceFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```