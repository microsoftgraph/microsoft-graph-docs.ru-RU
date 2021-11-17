---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d17208adb53f915aad45ba8a98eb35439eb3b89
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "61020395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let softwareOathAuthenticationMethod = await client.api('/me/authentication/softwareOathMethods/b172893e-893e-b172-3e89-72b13e8972b1')
    .version('beta')
    .get();

```