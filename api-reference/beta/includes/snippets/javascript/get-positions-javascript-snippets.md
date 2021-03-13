---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 89357e65deadec856d421d372baeb2b9faa6d7ac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let positions = await client.api('/me/profile/positions')
    .version('beta')
    .get();

```