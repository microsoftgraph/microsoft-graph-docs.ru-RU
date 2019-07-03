---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fa0849edc7b30a91fdc2e048f852c3ef1c79fa3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489563"
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