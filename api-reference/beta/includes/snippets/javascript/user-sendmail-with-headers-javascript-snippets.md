---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 48b7389e6d99296542fb2061bd90c5de20ac590a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  message: {
    subject: '9/9/2018: concert',
    body: {
      contentType: 'HTML',
      content: 'The group represents Nevada.'
    },
    toRecipients: [
      {
        emailAddress: {
          address: 'AlexW@contoso.OnMicrosoft.com'
        }
      }
    ],
    internetMessageHeaders: [
      {
        name: 'x-custom-header-group-name',
        value: 'Nevada'
      },
      {
        name: 'x-custom-header-group-id',
        value: 'NV001'
      }
    ]
  }
};

await client.api('/me/sendMail')
    .version('beta')
    .post(sendMail);

```