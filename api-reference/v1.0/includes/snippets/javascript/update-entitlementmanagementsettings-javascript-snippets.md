---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f48552e8fb6d5dadcc9184dfee94fb084df87b8b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const entitlementManagementSettings = {
  externalUserLifecycleAction: 'None'
};

await client.api('/identityGovernance/entitlementManagement/settings')
    .update(entitlementManagementSettings);

```