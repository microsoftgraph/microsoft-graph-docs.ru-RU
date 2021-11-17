---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 40cf2499224734acfae2edbb34ee82ecdb6e1f19
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new AppleManagedIdentityProvider
{
    DisplayName = "Sign in with Apple",
    DeveloperId = "UBF8T346G9",
    ServiceId = "com.microsoft.rts.b2c.test.client",
    KeyId = "99P6D879C4",
    CertificateData = "******"
};

await graphClient.Identity.IdentityProviders
    .Request()
    .AddAsync(identityProviderBase);

```