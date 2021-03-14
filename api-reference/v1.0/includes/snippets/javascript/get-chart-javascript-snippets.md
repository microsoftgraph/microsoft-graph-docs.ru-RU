---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d54f10fde67d23f49bc850f7aed40e2337574caf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChart = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .get();

```