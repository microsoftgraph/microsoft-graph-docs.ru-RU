---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f41b9b2259b225df0bc447d10f0b0054ba68e180a63c55717bdf5df6d0771a39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57202746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt')
    .version('beta')
    .post(workbookTableColumn);

```