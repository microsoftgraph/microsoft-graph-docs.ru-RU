---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb9290c11769f3f3ebc2917050768a471ccddcd7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemEmail = {
  address: 'Innocenty.Popov@adventureworks.com',
};

await client.api('/me/profile/emails')
    .version('beta')
    .post(itemEmail);

```