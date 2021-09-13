---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8c64c2b13b09e278d6d5a585bda7b74e42f4a3ecda6dec1b0757653e441b84ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57311329"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
DefaultUserRolePermissions defaultUserRolePermissions = new DefaultUserRolePermissions();
LinkedList<String> permissionGrantPoliciesAssignedList = new LinkedList<String>();
permissionGrantPoliciesAssignedList.add("managePermissionGrantsForSelf.microsoft-user-default-low");
defaultUserRolePermissions.permissionGrantPoliciesAssigned = permissionGrantPoliciesAssignedList;
authorizationPolicy.defaultUserRolePermissions = defaultUserRolePermissions;

graphClient.policies().authorizationPolicy()
    .buildRequest()
    .patch(authorizationPolicy);

```