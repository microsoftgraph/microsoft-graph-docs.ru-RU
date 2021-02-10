---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 67ae7803b4ccf4b3025440cc1ee72c7b31e98061
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176248"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessPackageResourceEnvironmentCollectionPage accessPackageResourceEnvironments = graphClient.identityGovernance().entitlementManagement().accessPackageResourceEnvironments()
    .buildRequest()
    .filter("originSystem eq 'SharePointOnline'")
    .get();

```