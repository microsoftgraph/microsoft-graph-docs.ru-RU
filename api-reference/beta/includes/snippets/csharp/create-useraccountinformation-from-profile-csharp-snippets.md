---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e37aaa3a0477eeee308d37baddd7a3e74dc85451
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441029"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = new UserAccountInformation
{
    AllowedAudiences = AllowedAudiences.Organization,
    CountryCode = "NO"
};

await graphClient.Me.Profile.Account
    .Request()
    .AddAsync(userAccountInformation);

```