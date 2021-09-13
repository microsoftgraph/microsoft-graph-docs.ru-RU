---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31a57647b18cc028b85d0c17654959abf55ebbfdd591ecb84ab5cf9d18d74fa3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartFont = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font')
    .get();

```