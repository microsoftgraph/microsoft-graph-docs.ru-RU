---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e3a5209b6493625d8b9059454fbe530e45f94c63
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/users/{userId}/drives')
    .get();

```