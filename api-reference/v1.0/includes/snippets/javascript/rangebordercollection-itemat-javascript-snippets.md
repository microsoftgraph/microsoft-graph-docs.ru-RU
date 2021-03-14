---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1b0446ab1f7c5615e1f09b7b8a8c1309630319c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: 1
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt')
    .post(workbookRangeBorder);

```