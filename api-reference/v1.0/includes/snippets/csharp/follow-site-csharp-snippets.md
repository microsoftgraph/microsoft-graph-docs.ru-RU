---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d9d5546c3a7ef5f5ea7cf9fbb3b96270c67211e1
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<Site>()
{
    new Site
    {
        Id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
    },
    new Site
    {
        Id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
    }
};

await graphClient.Users["{user-id}"].FollowedSites
    .Add(value)
    .Request()
    .PostAsync();

```