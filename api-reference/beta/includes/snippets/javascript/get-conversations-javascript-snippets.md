---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1d0e51d40f9da9e337cf0b1d066190296d8c748c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversations = await client.api('/groups/{id}/conversations')
    .version('beta')
    .get();

```