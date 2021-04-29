---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 224e0cb3657c1234903de8266b66e20388c8de41
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081495"
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

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].IdentityProviders.References
    .Request()
    .AddAsync(identityProvider);

```