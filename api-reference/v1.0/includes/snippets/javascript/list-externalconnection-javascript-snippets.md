---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc6d62fbed067c228d5a2442e15756cba584fcd5
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connections = await client.api('/connections')
    .get();

```