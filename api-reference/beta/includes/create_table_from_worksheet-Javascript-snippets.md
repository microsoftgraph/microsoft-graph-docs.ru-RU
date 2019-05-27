---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fa0849edc7b30a91fdc2e048f852c3ef1c79fa3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: "",
  hasHeaders: false
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add')
    .version('beta')
    .post(workbookTable);

```