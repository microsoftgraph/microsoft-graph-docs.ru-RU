---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99cc4142fd1fc9a2f720615728a6f780de6fec97
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/businessFlowTemplates')
    .version('beta')
    .get();

```