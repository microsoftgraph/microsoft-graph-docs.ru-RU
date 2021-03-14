---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 259b5c4fb94adf191a84567df8fa6b70fe752c51
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alerts = await client.api('/security/alerts')
    .get();

```