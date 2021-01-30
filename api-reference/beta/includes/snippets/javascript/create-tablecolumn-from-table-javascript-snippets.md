---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 434485a2b4ba75a4370a055a174fc6d8ab0c1bf2
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  id: "99",
  name: "name-value",
  index: 99,
  values: "values-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .version('beta')
    .post(workbookTableColumn);

```