---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a44ed2c9b694504d95551bc68508e6b5d78c97a15a561514cf45bebd20b518d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scopedRoleMembership = {
  roleId: 'roleId-value',
  roleMemberInfo: {
    id: 'id-value'
  }
};

await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .post(scopedRoleMembership);

```