---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 59f9240c0b8657d115b10f01c2ae28fe9e652e812ac2056e3eba1feaa43943ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57249142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartDataLabels = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels')
    .get();

```