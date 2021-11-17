---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9b5eede9972dae6ca422c684f6e76184051838b445dfa2ca4d3911d2907d8a01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57315971"
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
    .version('beta')
    .update(entitlementManagementSettings);

```