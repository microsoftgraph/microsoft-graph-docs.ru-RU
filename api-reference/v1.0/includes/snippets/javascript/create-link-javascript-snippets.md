---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3dc82eba6c6ce59077d1ab5e9e5ef72a0efa7e4a47a4dc3200439eeb9fd6e1fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57055275"
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