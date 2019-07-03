---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 27ec6610634a2266c765361183657e87a9c1874d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns')
    .version('beta')
    .get();

```