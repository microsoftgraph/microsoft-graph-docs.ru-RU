---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 74cda10a84ec58bc514da43eb2a46ff06c695874
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identitySecurityDefaultsEnforcementPolicy = new IdentitySecurityDefaultsEnforcementPolicy
{
    IsEnabled = false
};

await graphClient.Policies.IdentitySecurityDefaultsEnforcementPolicy
    .Request()
    .UpdateAsync(identitySecurityDefaultsEnforcementPolicy);

```