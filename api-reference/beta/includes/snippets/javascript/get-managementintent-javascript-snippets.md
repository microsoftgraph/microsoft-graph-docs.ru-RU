---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7a58c8512e533ff9a4b521968bd9c7f1eb803841c811c30aa3d8c9d4b977ebd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57211766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementIntent = await client.api('/tenantRelationships/managedTenants/managementIntents/{managementIntentId}')
    .version('beta')
    .get();

```