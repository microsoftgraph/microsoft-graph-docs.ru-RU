---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99cc4142fd1fc9a2f720615728a6f780de6fec97
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529205"
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