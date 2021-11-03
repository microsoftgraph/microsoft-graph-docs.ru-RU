---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3c30517d157fd1f4f135c98e0659fa2eeb6c274b72ab87fc4b0bd7ab793b8544
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
  displayName: 'Access Package New Name'
};

await client.api('/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}')
    .version('beta')
    .update(accessPackage);

```