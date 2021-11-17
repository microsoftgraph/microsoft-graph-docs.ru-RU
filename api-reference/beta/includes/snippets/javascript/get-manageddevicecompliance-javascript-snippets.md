---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b1781a04020d6fbc6159eed5a19c53da6bbb9fc73c51455aac0799852180153
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57308112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managedDeviceCompliance = await client.api('/tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}')
    .version('beta')
    .get();

```