---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a8556b6309bb576114f2684afbbe8773caa0ae9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/chats/{id}/messages/{id}/replies')
    .version('beta')
    .get();

```