---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4b8a9874af8c23c112a880963b25689add4b40b2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35473800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicy = {
  groupLifetimeInDays: 100,
  managedGroupTypes: "Selected",
  alternateNotificationEmails: "admin@contoso.com"
};

let res = await client.api('/groupLifecyclePolicies')
    .post({groupLifecyclePolicy : groupLifecyclePolicy});

```