---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 085252dbd03a1b32b2dcc966a8c49a1bec0498cdec09913b13db4c8a9283680a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57192449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let apiConnectors = await client.api('/identity/apiConnectors')
    .version('beta')
    .get();

```