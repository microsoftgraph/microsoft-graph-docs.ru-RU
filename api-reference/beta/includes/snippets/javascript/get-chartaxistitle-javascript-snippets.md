---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9275678ac319d7ec663437766e20e8e6a2ed4732
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789760"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartAxisTitle = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title')
    .version('beta')
    .get();

```