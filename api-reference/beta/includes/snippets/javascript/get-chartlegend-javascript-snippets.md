---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 314a4906e1e4b741b5af966fc628ecc9154a7da070f81f6c4282eee1b1de88fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143586"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartLegend = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .version('beta')
    .get();

```