---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c99c2415f67375a1f0a3b0d4701f2ef735c501a4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741114"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartTitle = {
  overlay: true,
  text: "text-value",
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .update({workbookChartTitle : workbookChartTitle});

```