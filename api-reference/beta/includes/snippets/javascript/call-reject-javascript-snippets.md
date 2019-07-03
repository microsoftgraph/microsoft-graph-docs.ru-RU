---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 214c0a91ee4ab17c0f480c2c40992e6b2602554e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528443"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: "none"
};

let res = await client.api('/app/calls/{id}/reject')
    .version('beta')
    .post(reject);

```