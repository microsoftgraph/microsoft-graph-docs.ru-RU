---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9201c1fb9f1790c447113dcf81e268cdfea10663b9531ffbebffb62fc1d1fd7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethod = await client.api('/me/authentication/methods/{id}')
    .version('beta')
    .get();

```