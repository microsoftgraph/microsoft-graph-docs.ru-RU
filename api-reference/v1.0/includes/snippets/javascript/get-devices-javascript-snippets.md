---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0bd7b6b87cfeac5424e4ae130df6433a105a226c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices')
    .get();

```