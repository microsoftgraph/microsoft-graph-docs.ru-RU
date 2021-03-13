---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 752fe863889051e678d39029f6849447ad12e3e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/AAMkAGVmMDEzM/childFolders')
    .version('beta')
    .get();

```