---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c5bbf7bf64008a178af825c225240744c5132a46
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLegend = {
  visible: true,
  position: "position-value",
  overlay: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .version('beta')
    .update({workbookChartLegend : workbookChartLegend});

```