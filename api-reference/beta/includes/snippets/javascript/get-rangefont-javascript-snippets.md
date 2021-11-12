---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c97b08f0fb9639116dc804f9947169512ba37a826f05ad43346d09253d497b70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57320024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFont = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/font')
    .version('beta')
    .get();

```