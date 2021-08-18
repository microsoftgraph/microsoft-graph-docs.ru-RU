---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4e927ce735be83df0bf1303d154fe185b9037ba8
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258903"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppManagementPolicy appManagementPolicy = new AppManagementPolicy();
appManagementPolicy.isEnabled = false;

graphClient.policies().appManagementPolicies("{id}")
    .buildRequest()
    .patch(appManagementPolicy);

```