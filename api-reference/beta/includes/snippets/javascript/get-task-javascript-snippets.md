---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2fbd6d38fc6ed1c165bfa39c2d7c0e5a726ded0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTask = await client.api('/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3')
    .version('beta')
    .get();

```