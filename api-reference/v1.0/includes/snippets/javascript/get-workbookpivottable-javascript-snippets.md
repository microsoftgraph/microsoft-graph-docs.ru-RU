---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bade9f9b2c78e14c2bcedc1f10fd223e9439e5fa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookPivotTable = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}')
    .get();

```