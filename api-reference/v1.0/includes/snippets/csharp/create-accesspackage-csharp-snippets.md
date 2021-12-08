---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb9f584ab9362736ab2f79093844bbe876101c5b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackage = new AccessPackage
{
    DisplayName = "sales reps",
    Description = "outside sales representatives",
    IsHidden = false,
    Catalog = new AccessPackageCatalog
    {
        Id = "66584aae-98bb-48cc-9458-7bee5d2a6577"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .Request()
    .AddAsync(accessPackage);

```