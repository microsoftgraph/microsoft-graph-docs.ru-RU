---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cfb6fb95f44a4285f7b67c3a730ba562bc928de4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778612"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personName = await client.api('/me/profile/names/{id}')
    .version('beta')
    .get();

```