---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a0dcf7497331cc508635e6798c4bc6545f46e16cd3f642928d7e7af5eefaeeb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identityProviders/{id}"}
    }
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].IdentityProviders.References
    .Request()
    .AddAsync(identityProvider);

```