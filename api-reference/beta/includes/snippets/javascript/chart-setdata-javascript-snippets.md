---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3669f1a50b83709e3f2b9612e0b9838b61b4ecad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setData = {
  sourceData: 'sourceData-value',
  seriesBy: 'seriesBy-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData')
    .version('beta')
    .post(setData);

```