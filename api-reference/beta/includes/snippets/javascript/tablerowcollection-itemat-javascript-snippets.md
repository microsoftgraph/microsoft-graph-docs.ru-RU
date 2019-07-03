---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d5cc4cf513e4f14f0307938818832f932ee69fc2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt')
    .version('beta')
    .post({workbookTableRow : workbookTableRow});

```