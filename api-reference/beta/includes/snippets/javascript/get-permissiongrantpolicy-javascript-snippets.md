---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 55f105ed3ca8fd6927479c0b7c3d10df86ec913e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrantPolicy = await client.api('/policies/permissionGrantPolicies/microsoft-user-default-low')
    .version('beta')
    .get();

```