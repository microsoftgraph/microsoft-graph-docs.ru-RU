---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: de1a6c08eec47c7a0256c22a1f458affe4aecbcf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976416"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlow identityUserFlow = new IdentityUserFlow();
identityUserFlow.id = "Pol1";
identityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
identityUserFlow.userFlowTypeVersion = 1;

graphClient.identity().userFlows()
    .buildRequest()
    .post(identityUserFlow);

```