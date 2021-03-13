---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 20bd469893972cae4658e5946ad04321dc5d6731
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805866"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workPosition = await client.api('/me/profile/positions/{id}')
    .version('beta')
    .get();

```