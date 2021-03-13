---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ac6625dd97f928a31bb68c126469e864203cfbd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResourceEnvironments = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceEnvironments')
    .version('beta')
    .filter('originSystem eq \'SharePointOnline\'')
    .get();

```