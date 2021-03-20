---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a67096e1081cee6b1674d62c50c53a5d679fc6bc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  name: 'test5',
  reference: '=Sheet1!$F$15:$N$27',
  comment: 'Comment for the named item'
};

await client.api('/me/drive/items/{id}/workbook/names/add')
    .post(workbookNamedItem);

```