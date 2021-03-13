---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b68288026af04df8d696beaea3d1856e1ad9f33
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: 'Annual review',
  body: {
    contentType: 'HTML',
    content: 'You should be proud!'
  },
  toRecipients: [
    {
      emailAddress: {
        address: 'rufus@contoso.com'
      }
    }
  ],
  extensions: [
    {
      '@odata.type': 'microsoft.graph.openTypeExtension',
      extensionName: 'Com.Contoso.Referral',
      companyName: 'Wingtip Toys',
      expirationDate: '2015-12-30T11:00:00.000Z',
      dealValue: 10000
    }
  ]
};

await client.api('/me/messages')
    .version('beta')
    .post(message);

```