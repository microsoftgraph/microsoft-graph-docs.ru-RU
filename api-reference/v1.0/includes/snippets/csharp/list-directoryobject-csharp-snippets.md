---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 034cf81c7bef94e7b1804a01b4f28c8af07e7aab
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62138226"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var internalSponsors = await graphClient.IdentityGovernance.EntitlementManagement.Assignments["{accessPackageAssignment-id}"].Target.ConnectedOrganization.InternalSponsors
    .Request()
    .GetAsync();

```