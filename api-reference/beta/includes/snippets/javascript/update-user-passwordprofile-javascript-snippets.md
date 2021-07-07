---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b5a4bc0dcb8f39db3c93e957b1997365230e44b
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  passwordProfile: {
    forceChangePasswordNextSignIn: false,
    password: 'xWwvJ]6NMw+bWH-d'
  }
};

await client.api('/users/{id}')
    .version('beta')
    .update(user);

```