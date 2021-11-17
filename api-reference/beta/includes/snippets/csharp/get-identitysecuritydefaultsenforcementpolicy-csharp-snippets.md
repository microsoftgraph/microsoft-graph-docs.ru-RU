---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 41f1fab84d826e1bb0435a0c7f11c55c098bd6bed1e515ad107faaf43997b5ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57198769"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identitySecurityDefaultsEnforcementPolicy = await graphClient.Policies.IdentitySecurityDefaultsEnforcementPolicy
    .Request()
    .GetAsync();

```