---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eddf334e15c58a42f961d03f4a7f94443ed13db3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35473777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: 1
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt')
    .post({workbookRangeBorder : workbookRangeBorder});

```