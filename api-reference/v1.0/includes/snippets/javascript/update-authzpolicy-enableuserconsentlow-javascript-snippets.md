---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1d1a4a2129d0b6fffe66ff7e0faaba283422bfe0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   defaultUserRolePermissions: {
      permissionGrantPoliciesAssigned: [
         'managePermissionGrantsForSelf.microsoft-user-default-low'
      ]
   }
};

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```