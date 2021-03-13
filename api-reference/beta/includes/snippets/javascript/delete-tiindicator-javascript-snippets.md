---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eeb36c5837751afe0fc1299613a88bee8d771725
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787205"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .delete();

```