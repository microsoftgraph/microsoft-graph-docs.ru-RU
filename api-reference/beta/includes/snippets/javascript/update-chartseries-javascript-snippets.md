---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0736d8d4606c6c5cf7d40c1a5966e03af8a70abe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}')
    .version('beta')
    .update({workbookChartSeries : workbookChartSeries});

```