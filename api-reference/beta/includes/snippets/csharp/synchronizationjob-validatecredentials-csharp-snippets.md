---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ca59ca1b3256fb80a5d23c351febbb756579dd5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773573"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentials = new List<SynchronizationSecretKeyStringValuePair>()
{
    new SynchronizationSecretKeyStringValuePair
    {
        Key = SynchronizationSecret.UserName,
        Value = "user@domain.com"
    },
    new SynchronizationSecretKeyStringValuePair
    {
        Key = SynchronizationSecret.Password,
        Value = "password-value"
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .ValidateCredentials(null,null,null,credentials)
    .Request()
    .PostAsync();

```