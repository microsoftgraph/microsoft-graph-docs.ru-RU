---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99a4d2260adb897c8732a4d48a32021ed0e206cd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: "Sheet1!A1:D5",
  hasHeaders: true
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/add')
    .version('beta')
    .post(workbookTable);

```