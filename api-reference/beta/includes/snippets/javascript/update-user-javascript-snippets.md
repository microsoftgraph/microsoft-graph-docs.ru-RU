---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2fd9faa3a78438b9994a6b06c279e05ffaf00cb3f8daedc4978a8a154dbd2303
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57370187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    '+1 425 555 0109'
  ],
  officeLocation: '18/2111'
};

await client.api('/me')
    .version('beta')
    .update(user);

```