---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96f444f113f21d30f912025fecd1f72bac95425c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: '#00FF00'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill')
    .version('beta')
    .update(workbookRangeFill);

```