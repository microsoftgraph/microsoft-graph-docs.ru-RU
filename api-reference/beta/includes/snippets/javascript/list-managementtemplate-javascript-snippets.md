---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4dc781a07d8ed39e0888fe6bc61d8be7b3c8b9362ed3012a73d8e1e01da1523a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementTemplates = await client.api('/tenantRelationships/managedTenants/managementTemplates')
    .version('beta')
    .get();

```