---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ac9450a9c8b5633b7e4f9136a31356427976a840
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .version('beta')
    .skiptoken('c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA=')
    .get();

```