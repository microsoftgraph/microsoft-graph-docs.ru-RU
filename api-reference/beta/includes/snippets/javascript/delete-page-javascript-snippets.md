---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 879b167e7096f06226f2718a6f98653137c22e44
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/onenote/pages/{id}')
    .version('beta')
    .delete();

```