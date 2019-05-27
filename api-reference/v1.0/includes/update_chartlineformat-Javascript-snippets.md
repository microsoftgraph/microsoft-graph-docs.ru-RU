---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cfb0d39e4deb7b97c75d703ab70fe71ef1cc6c36
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLineFormat = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line')
    .update({workbookChartLineFormat : workbookChartLineFormat});

```