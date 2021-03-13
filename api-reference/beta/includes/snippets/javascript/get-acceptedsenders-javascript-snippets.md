---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bd983b0ba6e06e9700b603cf02680bc91341385f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acceptedSenders = await client.api('/groups/{id}/acceptedSenders')
    .version('beta')
    .get();

```