---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7dddeb006814e7662de62badf41a0a170aa818a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onenoteOperation = await client.api('/me/onenote/operations/{id}')
    .version('beta')
    .get();

```