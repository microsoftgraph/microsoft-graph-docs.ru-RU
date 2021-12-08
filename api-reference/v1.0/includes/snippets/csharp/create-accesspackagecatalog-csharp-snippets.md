---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 08d490ed0f261e262be20679c4aeb944a99ce998
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = new AccessPackageCatalog
{
    DisplayName = "sales",
    Description = "for employees working with sales and outside sales partners",
    State = AccessPackageCatalogState.Published,
    IsExternallyVisible = true
};

await graphClient.IdentityGovernance.EntitlementManagement.Catalogs
    .Request()
    .AddAsync(accessPackageCatalog);

```