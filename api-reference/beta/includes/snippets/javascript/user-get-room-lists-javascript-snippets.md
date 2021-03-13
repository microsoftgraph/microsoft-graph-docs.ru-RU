---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 53021a088ccfbbfc1089249a3abe4d6425d2e125
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let findRoomLists = await client.api('/me/findRoomLists')
    .version('beta')
    .get();

```