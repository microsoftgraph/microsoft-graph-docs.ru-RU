---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8d9d9a0540cce225874500dc76e3e456278f750d792b9d772ef83da21b43c5c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}')
    .version('beta')
    .delete();

```