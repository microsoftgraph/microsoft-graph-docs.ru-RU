---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 551e6768e28c19e4430cba1e843203b3519b965aa7b5d4514b980f2a9b141eeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignments
    .FilterByCurrentUser(AccessPackageAssignmentFilterByCurrentUserOptions.Target)
    .Request()
    .GetAsync();

```