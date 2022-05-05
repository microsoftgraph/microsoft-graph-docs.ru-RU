---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d7fa39e103deb992973657305691f3b15d46eb8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211798"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var internalDomainFederation = new InternalDomainFederation
{
    DisplayName = "Contoso name change",
    FederatedIdpMfaBehavior = FederatedIdpMfaBehavior.AcceptIfMfaDoneByFederatedIdp
};

await graphClient.Domains["{domain-id}"].FederationConfiguration["{internalDomainFederation-id}"]
    .Request()
    .UpdateAsync(internalDomainFederation);

```