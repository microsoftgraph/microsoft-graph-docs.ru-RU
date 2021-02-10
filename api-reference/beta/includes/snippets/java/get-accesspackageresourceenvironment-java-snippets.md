---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7598b1257f79b1f822f299fe063b10cbc6642251
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176304"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceEnvironment accessPackageResourceEnvironment = graphClient.identityGovernance().entitlementManagement().accessPackageResourceEnvironments("{accessPackageResourceEnvironmentId}")
    .buildRequest()
    .get();

```