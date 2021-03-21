---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ff0071695104c0874f1e5a7576afccca4f06512
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookTask = await client.api('/me/outlook/tasks/AAMkADA1MHgwAAA=')
    .version('beta')
    .header('Prefer','outlook.timezone="Pacific Standard Time"')
    .get();

```