---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3023b55e92074833b0373f5e7b0444fc53aee184
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleInstances
    .FilterByCurrentUser(RoleEligibilityScheduleInstanceFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```