---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 651d093425a570245ad0ef570a0cf9fc2fda6882
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/deletedItems/{object-id}/restore')
    .post();

```