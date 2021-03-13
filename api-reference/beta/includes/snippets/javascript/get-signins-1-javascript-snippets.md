---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b5c4630d87c26460928951f672444cb37ac38f03
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signIns')
    .version('beta')
    .get();

```