---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b98883f776fec951fcf964500da56397b26203e3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .skip(5)
    .top(5)
    .get();

```