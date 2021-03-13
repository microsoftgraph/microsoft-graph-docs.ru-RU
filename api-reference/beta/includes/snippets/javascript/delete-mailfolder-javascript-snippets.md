---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c400c3508ae59497692faba1eaf9e63f38ceb275
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailFolders/AAMkAGVmMDEzM/')
    .version('beta')
    .delete();

```