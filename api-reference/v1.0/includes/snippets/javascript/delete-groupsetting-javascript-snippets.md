---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e7a96368b0ad11c854e02e4ae5b109f5810f5d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groupSettings/{id}')
    .delete();

```