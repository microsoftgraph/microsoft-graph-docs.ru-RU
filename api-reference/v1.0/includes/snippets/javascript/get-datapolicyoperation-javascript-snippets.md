---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ee7a15fdbca1cabe3228a998a99ef5611eb2e7f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/dataPolicyOperations/{id}')
    .get();

```