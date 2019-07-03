---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8271891c1fd6931316c0f0e561ed0fe38754507d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  type: "type-value",
  scope: "scope-value",
  comment: "comment-value",
  value: {
  },
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .update({workbookNamedItem : workbookNamedItem});

```