---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9725a47e7e012ef6610d4dc632b1b86e034d2107
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableColumn = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .version('beta')
    .get();

```