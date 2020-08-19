---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 80628ed52a5df47bb5780f4ee0f1228c6a6e91fd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
  displayName:"Access Package New Name"
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}')
    .version('beta')
    .update(accessPackage);

```