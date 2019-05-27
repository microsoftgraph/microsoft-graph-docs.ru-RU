---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 227e6974ede1fed740a1e4e77c4862f3fed9fcd4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
  address: "address-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/Range')
    .version('beta')
    .post(workbookRange);

```