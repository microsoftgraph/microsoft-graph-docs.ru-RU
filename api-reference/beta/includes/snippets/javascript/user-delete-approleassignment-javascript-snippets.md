---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 30d8aecff103d48c4d1ff6063be1b22033f148abb1927f550f6bae0c5b2491e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57263290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id}/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```