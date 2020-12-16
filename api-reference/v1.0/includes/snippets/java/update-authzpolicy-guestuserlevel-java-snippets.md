---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7737a8c3384b22929033232a3e3c20e258b5c263
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691464"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
authorizationPolicy.allowEmailVerifiedUsersToJoinOrganization = false;

graphClient.policies().authorizationPolicy()
    .buildRequest()
    .patch(authorizationPolicy);

```