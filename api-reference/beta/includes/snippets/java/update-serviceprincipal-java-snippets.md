---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 979ae76ee73f57133bdcb786f51b7cf477c3e450bb5211e6099b4a90cd0d2241
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052354"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appRoleAssignmentRequired = true;

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .patch(servicePrincipal);

```