---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2b6a3f9b4b0240d1d6bd7f4210c7282c7040a0a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scopedRoleMembership = {
  roleId: "roleId-value",
  roleMemberInfo: {
    id: "id-value"
  }
};

let res = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .post({scopedRoleMembership : scopedRoleMembership});

```