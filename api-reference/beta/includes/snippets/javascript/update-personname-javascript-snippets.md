---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b0a7595d61da46427962ca0d5775d80bf643990
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personName = {
  nickname: 'Kesha'
};

await client.api('/me/profile/names/{id}')
    .version('beta')
    .update(personName);

```