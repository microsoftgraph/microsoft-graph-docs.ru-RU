---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc49c3b40ddbfb2b21cdc70aed849c4afa92ac87
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: [ 'read' ]
};

await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .update(permission);

```