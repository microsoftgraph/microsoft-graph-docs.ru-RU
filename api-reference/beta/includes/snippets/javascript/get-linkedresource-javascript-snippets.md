---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 02d66ddff03ac4bb069b9ed43273f467a7ccfb68
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let linkedResource = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9')
    .version('beta')
    .get();

```