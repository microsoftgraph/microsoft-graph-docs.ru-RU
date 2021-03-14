---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 122c346e6cd17d54480efb0478671da5d24accb6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let createdObjects = await client.api('/me/createdObjects')
    .get();

```