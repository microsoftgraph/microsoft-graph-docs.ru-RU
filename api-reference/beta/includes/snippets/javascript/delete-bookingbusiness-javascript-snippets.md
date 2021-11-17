---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5080a9bd3bd5b552c4230ac0a543118e13893815a86391ae0c16599f92cf664d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57197951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com')
    .version('beta')
    .delete();

```