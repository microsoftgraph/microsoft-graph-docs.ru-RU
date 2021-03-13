---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 75f85fab4e741ecb16690e0d126434735e2cd597
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const webAccount = {
  webUrl: 'https://github.com/innocenty.popov'
};

await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .update(webAccount);

```