---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b87c8b4e56d51f886cc1efd1a3f03df52f0dfd57
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicy = {
  groupLifetimeInDays: 180,
  managedGroupTypes: "Selected",
  alternateNotificationEmails: "admin@contoso.com"
};

let res = await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .update({groupLifecyclePolicy : groupLifecyclePolicy});

```