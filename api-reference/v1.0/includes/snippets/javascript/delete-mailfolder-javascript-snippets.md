---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fb3f93f2c881185e7482395da09f9e4a9994d57fa42e6efd25436ab52afc1bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57191592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailFolders/{id}')
    .delete();

```