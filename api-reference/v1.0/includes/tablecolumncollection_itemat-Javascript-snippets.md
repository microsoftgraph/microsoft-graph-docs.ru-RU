---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 13adc7c6b052a947a956baf4eefcc9eb92d96dc3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449963"
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