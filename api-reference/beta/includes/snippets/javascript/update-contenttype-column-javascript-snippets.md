---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 949e6de41ad29df4b7de5b26170bd25996d501b0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const columnDefinition = {
  required: true,
  hidden: false,
  propagateChanges: false       
};

await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .version('beta')
    .update(columnDefinition);

```