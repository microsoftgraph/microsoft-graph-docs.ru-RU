---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb40f248555b22ac2d4440f3c82970778b0b2037
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/schools')
    .get();

```