---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aeb6d527bc579bcdab4653a8fee70829cc397d39ffb95a6897e8d43c435ed18d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var approval = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"]
    .Request()
    .GetAsync();

```