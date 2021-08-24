---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 94557f2a966d6bb48af66cda169fda16f470d2e3db685d8c95a5eebeb21dfff6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57373931"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.displayName = "Password friendly name";

graphClient.servicePrincipals("{id}")
    .addPassword(ServicePrincipalAddPasswordParameterSet
        .newBuilder()
        .withPasswordCredential(passwordCredential)
        .build())
    .buildRequest()
    .post();

```