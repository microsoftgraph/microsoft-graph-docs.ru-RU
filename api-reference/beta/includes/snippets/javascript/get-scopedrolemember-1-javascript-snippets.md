---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 890be5a9d541d0e2aad29131a2ea56a78d504f9146e26aa24eb2dd1378858672
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembership = await client.api('/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .version('beta')
    .get();

```