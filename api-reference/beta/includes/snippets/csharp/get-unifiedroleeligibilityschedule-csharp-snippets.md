---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3678b1d32cdd6fee3cb6fccf2d7bcffdff40e6f8a2b5e71f6dc874cf3b794025
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilitySchedule = await graphClient.RoleManagement.Directory.RoleEligibilitySchedules["{unifiedRoleEligibilitySchedule-id}"]
    .Request()
    .GetAsync();

```