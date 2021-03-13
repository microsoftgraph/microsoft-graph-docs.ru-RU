---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 08c3f173b422a7e3f38651b3e15d5f9c9d9b679e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/termStore/sets/{setId}')
    .version('beta')
    .delete();

```