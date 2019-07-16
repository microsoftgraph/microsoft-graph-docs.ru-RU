---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 13adc7c6b052a947a956baf4eefcc9eb92d96dc3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt')
    .post({workbookTableColumn : workbookTableColumn});

```