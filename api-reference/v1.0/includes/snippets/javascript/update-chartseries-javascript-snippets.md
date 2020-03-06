---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6eb65e0795faddd9b072eab1638242befb173182
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}')
    .update(workbookChartSeries);

```