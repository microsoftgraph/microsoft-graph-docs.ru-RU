---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79befccd0bd7962b7c3d67ea21edf2ecb6d46907
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnniversary = {
  allowedAudiences: "contacts"
};

let res = await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .update(personAnniversary);

```