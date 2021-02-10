---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 62d3373fd07d997c76d35eafaec958168a490549
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176314"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}')
    .version('beta')
    .get();

```