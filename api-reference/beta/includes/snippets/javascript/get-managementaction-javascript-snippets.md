---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a97957e04a72a2f753e800eb6db6ea017d233d37e9df7996014991dca1ec7a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143083"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementAction = await client.api('/tenantRelationships/managedTenants/managementActions/{managementActionId}')
    .version('beta')
    .get();

```