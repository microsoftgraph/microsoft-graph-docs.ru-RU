---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 43d1cc1a9c34a2868a5fb77e877e851c80f339a6c6c5d8cbef4a73ea7c89e739
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57321499"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordAuthenticationMethod = await client.api('/me/authentication/passwordMethods/{id}')
    .version('beta')
    .get();

```