---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0920befbd44ce6c8aaf94592e08393dcae201da3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787942"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  '@odata.id': 'https://graph.microsoft.com/beta/users/{id}'
};

await client.api('/print/shares/{id}/allowedUsers/$ref')
    .version('beta')
    .post(user);

```