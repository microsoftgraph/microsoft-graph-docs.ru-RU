---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5006b8caec87f665dbb93c6ec1f6f117a858d7e0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appManagementPolicy = {
    isEnabled: false
};

await client.api('/policies/appManagementPolicies/{id}')
    .version('beta')
    .update(appManagementPolicy);

```