---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c0316f299cc49c856fe52bae287e3460de7855bd
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const entitlementManagementSettings = {
  externalUserLifecycleAction: "None"
};

let res = await client.api('/identityGovernance/entitlementManagement/settings')
    .version('beta')
    .update(entitlementManagementSettings);

```