---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3fcad8c5f36dc5420db5214be1dd40c69cb1f850
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976468"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceEnvironment accessPackageResourceEnvironment = graphClient.identityGovernance().entitlementManagement().accessPackageResourceEnvironments("{accessPackageResourceEnvironmentId}")
    .buildRequest()
    .get();

```