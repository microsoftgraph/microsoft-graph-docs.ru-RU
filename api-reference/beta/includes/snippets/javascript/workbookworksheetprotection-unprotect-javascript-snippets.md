---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d99de14dd17aa0a05db6c18755ff8b1a63393c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unprotect = {
  password: 'password-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect')
    .version('beta')
    .post(unprotect);

```