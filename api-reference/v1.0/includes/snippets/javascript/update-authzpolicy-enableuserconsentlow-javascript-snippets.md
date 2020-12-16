---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc6d24ab2edd512f5b2289f19606b7d0ce60aee1
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   defaultUserRolePermissions: {
      permissionGrantPoliciesAssigned: [
         "managePermissionGrantsForSelf.microsoft-user-default-low"
      ]
   }
};

let res = await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```