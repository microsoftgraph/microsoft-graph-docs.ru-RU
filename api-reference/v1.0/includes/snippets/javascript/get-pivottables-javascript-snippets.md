---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3962aedcadad9a9e77a53f762da55ee925f0154a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let pivotTables = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables')
    .get();

```