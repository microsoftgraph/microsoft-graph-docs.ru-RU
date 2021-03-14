---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2256ad0ac23affcfa4f82932c6d7dde900b081c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableSort = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort')
    .get();

```