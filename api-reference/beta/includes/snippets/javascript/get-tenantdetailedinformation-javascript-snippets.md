---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 790ef9e67380e13932ab4b0b24022c3106025189a55c81213ea1339c3696ec31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57247412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantDetailedInformation = await client.api('/tenantRelationships/managedTenants/tenantsDetailedInformation/{tenantDetailedInformationId}')
    .version('beta')
    .get();

```