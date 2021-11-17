---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee55bdcc203e439a6dc9744aa6e7664ee24979c4e7a72ad28a6991d80c146043
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResources = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources')
    .version('beta')
    .filter('resourceType eq \'Application\'')
    .expand('accessPackageResourceScopes')
    .get();

```