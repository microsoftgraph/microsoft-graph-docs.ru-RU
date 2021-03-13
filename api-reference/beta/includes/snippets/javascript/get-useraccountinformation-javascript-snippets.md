---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c906c0aefa5795cba5e38de434963447e9f22946
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAccountInformation = await client.api('/me/profile/account/{id}')
    .version('beta')
    .get();

```