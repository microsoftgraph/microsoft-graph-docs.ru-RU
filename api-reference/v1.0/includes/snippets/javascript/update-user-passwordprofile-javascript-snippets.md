---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d48fb3ab36880d376ed338612eb1867397c7b525e127a9480ddbc57a7d92e1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57192904"
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
    .update(user);

```