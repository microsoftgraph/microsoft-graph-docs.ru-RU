---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff6ddc0ee318d09bbdea25a49afc6eb98c73f4ce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/userFlowAttributes/{id}')
    .version('beta')
    .delete();

```