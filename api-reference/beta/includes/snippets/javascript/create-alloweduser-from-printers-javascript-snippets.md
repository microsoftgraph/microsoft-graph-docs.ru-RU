---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 245c4c5a92be2c0bf156de5cc20c9dc038961f11518cf9444a828abd6fdb1cc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57362091"
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