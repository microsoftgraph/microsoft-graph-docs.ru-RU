---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 75548121e7873bd556afbdd57a3e502863c8445b65435cf19bd9fba3a34e1ea6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316752"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartFont = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font')
    .version('beta')
    .get();

```