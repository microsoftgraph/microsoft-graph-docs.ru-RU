---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a223867a0391dd7f3ba683792256405ce2f0889
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreementAcceptances = await client.api('/me/agreementAcceptances')
    .get();

```