---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe6a229e1b2adb92ac892d23d401b62413421aea3d83c0cdb05dd96c59406595
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57264271"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .version('beta')
    .get();

```