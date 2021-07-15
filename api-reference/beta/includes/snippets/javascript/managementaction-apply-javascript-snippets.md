---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0235007d923068529a18413f29659cc09e37e6c0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const managementActionDeploymentStatus = {
  tenantId: 'String',
  tenantGroupId: 'String',
  managementTemplateId: 'String'
};

await client.api('/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply')
    .version('beta')
    .post(managementActionDeploymentStatus);

```