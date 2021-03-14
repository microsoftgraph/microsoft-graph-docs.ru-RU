---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 388c259659559461ed8820c1bb2a11383a671a07
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear')
    .post();

```