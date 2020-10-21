---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a2d86e716a423ed128ed2a5f7ee75e4130a10327
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts')
    .get();

```