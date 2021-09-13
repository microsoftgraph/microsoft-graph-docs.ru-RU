---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 021da219322515ee5175aec89c49dee4114073f71fa87c0c19076060eb4ca05f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57431233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartLegend = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .get();

```