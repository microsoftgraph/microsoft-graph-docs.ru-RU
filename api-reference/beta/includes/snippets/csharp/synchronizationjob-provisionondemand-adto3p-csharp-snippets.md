---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14e96df1875a5c3f08c3158d6632d8ca7e1f7da5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parameters = new List<SynchronizationJobApplicationParameters>()
{
    new SynchronizationJobApplicationParameters
    {
        Subjects = new List<SynchronizationJobSubject>()
        {
            new SynchronizationJobSubject
            {
                ObjectId = "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
                ObjectTypeName = "User"
            }
        },
        RuleId = "ea807875-5618-4f0a-9125-0b46a05298ca"
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .ProvisionOnDemand(parameters)
    .Request()
    .PostAsync();

```