---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eb5c3f2da5b951f2c07f41041ee3e378a2d80afc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969917"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectedOrganization connectedOrganization = new ConnectedOrganization();
connectedOrganization.displayName = "Connected organization new name";
connectedOrganization.description = "Connected organization new description";
connectedOrganization.state = ConnectedOrganizationState.CONFIGURED;

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}")
    .buildRequest()
    .patch(connectedOrganization);

```