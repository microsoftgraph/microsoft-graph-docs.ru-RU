---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5131efdb22e0478f8446e37976d764be6fb86a81
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61544966"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{connectedOrganizationId}").externalSponsors("{id}").reference()
    .buildRequest()
    .delete();

```