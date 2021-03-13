---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a639cc8ac4675eb5c32eb7be81b10d98c952a539
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFormat = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format')
    .version('beta')
    .get();

```