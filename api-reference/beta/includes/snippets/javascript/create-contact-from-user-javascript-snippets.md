---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2126f53637b68ce2f80c32a3ab4101bad84e890e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  givenName: 'Pavel',
  surname: 'Bansky',
  emailAddresses: [
    {
      address: 'pavelb@contoso.onmicrosoft.com',
      name: 'Pavel Bansky',
      type: 'personal'
    },
    {
      address: 'pavelb@fabrikam.onmicrosoft.com',
      name: 'Pavel Bansky',
      type: 'other',
      otherLabel: 'Volunteer work'
    }
  ],
  phones: [
    {
      number: '+1 732 555 0102',
      type: 'business'
    }
  ]
};

await client.api('/me/contacts')
    .version('beta')
    .post(contact);

```