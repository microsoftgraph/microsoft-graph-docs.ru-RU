---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ae10a079bee4049101532661d347bb8c7cf91a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/{id}/conversations/{id}/threads')
    .version('beta')
    .get();

```