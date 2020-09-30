---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e5588035d1b02845f4ee014b5ebfa8d3acc25b90
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48317974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganization = new ConnectedOrganization
{
    DisplayName = "Connected organization name",
    Description = "Connected organization description",
    IdentitySources = new List<IdentitySource>()
    {
        new DomainIdentitySource
        {
            DomainName = "example.com",
            DisplayName = "example.com"
        }
    },
    State = ConnectedOrganizationState.Proposed
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations
    .Request()
    .AddAsync(connectedOrganization);

```