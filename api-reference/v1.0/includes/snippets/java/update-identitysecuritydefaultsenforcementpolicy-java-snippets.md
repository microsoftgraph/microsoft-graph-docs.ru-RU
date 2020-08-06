---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d3f3c4a4a9a948a9b8513111a38dfa8fef78602
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567254"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentitySecurityDefaultsEnforcementPolicy identitySecurityDefaultsEnforcementPolicy = new IdentitySecurityDefaultsEnforcementPolicy();
identitySecurityDefaultsEnforcementPolicy.isEnabled = false;

graphClient.policies().identitySecurityDefaultsEnforcementPolicy()
    .buildRequest()
    .patch(identitySecurityDefaultsEnforcementPolicy);

```