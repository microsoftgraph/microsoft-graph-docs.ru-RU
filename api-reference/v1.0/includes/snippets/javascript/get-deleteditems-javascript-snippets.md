---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 593f3ed6b6b821dc48fd8bd60dbbab0f208fe9d0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/microsoft.graph.group')
    .get();

```