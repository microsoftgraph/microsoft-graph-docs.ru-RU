---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bf2e1b874ccbada9a43ac67aaee7a532d3079a79
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyCredential = new KeyCredential
{
    Type = "AsymmetricX509Cert",
    Usage = "Verify",
    Key = Convert.FromBase64String("MIIDYDCCAki...")
};

PasswordCredential passwordCredential = null;

var proof = "eyJ0eXAiOiJ...";

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .AddKey(keyCredential,proof,passwordCredential)
    .Request()
    .PostAsync();

```