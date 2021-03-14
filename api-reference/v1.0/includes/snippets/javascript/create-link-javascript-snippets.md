---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 582afd513c43182b264ddf98fcad7449412e5bc6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'view',
  password: 'ThisIsMyPrivatePassword',
  scope: 'anonymous'
};

await client.api('/me/drive/items/{item-id}/createLink')
    .post(permission);

```