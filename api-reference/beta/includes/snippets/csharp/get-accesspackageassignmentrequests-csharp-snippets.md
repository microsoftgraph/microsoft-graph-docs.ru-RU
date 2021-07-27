---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1cf9d3fe25656a849302bbcfbe81cfff91f3057
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequests = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .Filter("(requestState eq 'PendingApproval')")
    .Expand("requestor($expand=connectedOrganization)")
    .GetAsync();

```