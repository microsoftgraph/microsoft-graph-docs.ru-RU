---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 74cda10a84ec58bc514da43eb2a46ff06c695874
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947014"
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