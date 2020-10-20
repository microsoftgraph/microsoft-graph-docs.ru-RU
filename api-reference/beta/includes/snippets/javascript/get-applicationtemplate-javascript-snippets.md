---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee7b8bf37e7556c58e407807802ed5bb0e87cc72
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applicationTemplates/{id}')
    .version('beta')
    .get();

```