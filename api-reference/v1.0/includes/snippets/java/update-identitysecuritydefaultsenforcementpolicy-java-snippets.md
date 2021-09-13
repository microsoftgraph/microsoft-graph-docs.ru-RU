---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 90b849f3321d4f7ba8571e04c6958d29fde5cac772ed42da72cfe7aaf57e7944
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57365866"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentitySecurityDefaultsEnforcementPolicy identitySecurityDefaultsEnforcementPolicy = new IdentitySecurityDefaultsEnforcementPolicy();
identitySecurityDefaultsEnforcementPolicy.isEnabled = false;

graphClient.policies().identitySecurityDefaultsEnforcementPolicy()
    .buildRequest()
    .patch(identitySecurityDefaultsEnforcementPolicy);

```