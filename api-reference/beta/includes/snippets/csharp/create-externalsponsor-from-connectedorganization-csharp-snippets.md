---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 50eceeaa237bfbd82bd2b637824d198302c4bb4d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{id}"].ExternalSponsors.References
    .Request()
    .AddAsync(directoryObject);

```