---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c79d892d1c4197465c913bde2a15a8073da9d2a6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
  displayName: 'Notebook name'
};

await client.api('/me/onenote/notebooks')
    .version('beta')
    .post(notebook);

```