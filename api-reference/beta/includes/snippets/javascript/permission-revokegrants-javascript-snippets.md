---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c7c77e58df3ad3fc7604b4ebb7bc3e867d0c4af8d0c2ec6dc3b06bb238a737e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57260963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  grantees: [
    {
      email: 'ryan@contoso.com'
    }
  ]
};

await client.api('/me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants')
    .version('beta')
    .post(permission);

```