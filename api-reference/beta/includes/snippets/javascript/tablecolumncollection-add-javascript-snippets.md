---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 475ce5c481b000fd6750f2a2f6600751be46d1e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: {
  },
  values: [
    {
    }
  ]
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/add')
    .version('beta')
    .post(workbookTableColumn);

```