---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e446cb60c899b4eaa71d5dd4eda683b54404e7a1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  index: 8
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt')
    .post({workbookChart : workbookChart});

```