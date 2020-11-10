---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6f84ac259ad406ddb18a2a2793d93808ae868786
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961388"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationFlowsPolicy authenticationFlowsPolicy = new AuthenticationFlowsPolicy();
SelfServiceSignUpAuthenticationFlowConfiguration selfServiceSignUp = new SelfServiceSignUpAuthenticationFlowConfiguration();
selfServiceSignUp.isEnabled = true;
authenticationFlowsPolicy.selfServiceSignUp = selfServiceSignUp;

graphClient.policies().authenticationFlowsPolicy()
    .buildRequest()
    .patch(authenticationFlowsPolicy);

```