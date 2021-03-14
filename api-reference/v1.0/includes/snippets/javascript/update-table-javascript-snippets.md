---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ea856f02a89423c1215c3200e8c8e2537a203ffc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  name: 'name-value',
  showHeaders: true,
  showTotals: true,
  style: 'style-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .update(workbookTable);

```