---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e3b1b60487f61d140be00c7cc9b1c80210a00a0f
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335007"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = "principalId-value";
appRoleAssignment.resourceId = "resourceId-value";
appRoleAssignment.appRoleId = "appRoleId-value";

graphClient.servicePrincipals("{id}").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```