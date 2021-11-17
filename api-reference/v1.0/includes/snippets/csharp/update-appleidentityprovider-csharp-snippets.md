---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e46d83c5f2399160a55bd4aab7bbe7b78e8f598
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new IdentityProviderBase
{
    DisplayName = "Apple"
};

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .UpdateAsync(identityProviderBase);

```