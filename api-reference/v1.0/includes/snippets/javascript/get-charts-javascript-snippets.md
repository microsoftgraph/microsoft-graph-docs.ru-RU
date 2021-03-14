---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1756a5a1bf479a6d81426ccb85b5449d4290082e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let charts = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .get();

```