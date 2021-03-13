---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 08b3fecaeaeeee0f890797a2f1bf8e96a710ddb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPhone = {
  displayName: 'Car Phone',
  number: '+7 499 342 22 13'
};

await client.api('/me/profile/phones')
    .version('beta')
    .post(itemPhone);

```