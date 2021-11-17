---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8c53c9630ecececcbbf20f3e1a700320af0f9dc0c6ae2c942beab34cfd402332
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143379"
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