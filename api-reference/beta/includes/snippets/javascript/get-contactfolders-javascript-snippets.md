---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0a8b7a878bee5de4011a0fc5e1196fbc0e8aa7a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800799"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolders = await client.api('/me/contactFolders')
    .version('beta')
    .get();

```