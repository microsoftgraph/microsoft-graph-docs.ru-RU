---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ce018451b1cdbc901945c2d3527650230cdc48ad6cccd1bd9ea8af5db5c03eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57247252"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: 'john@contoso.com'
    },
    {
      email: 'ryan@external.com'
    }
  ],
  roles: ['read']
};

await client.api('/shares/{encoded-sharing-url}/permission/grant')
    .version('beta')
    .post(permission);

```