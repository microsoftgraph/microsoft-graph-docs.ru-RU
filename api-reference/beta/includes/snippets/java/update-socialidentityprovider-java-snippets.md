---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e3ee1641387919711f1c4d8e2088b553245267c8
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58369165"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SocialIdentityProvider identityProviderBase = new SocialIdentityProvider();
identityProviderBase.clientSecret = "1111111111111";

graphClient.identity().identityProviders("Amazon-OAUTH")
    .buildRequest()
    .patch(identityProviderBase);

```