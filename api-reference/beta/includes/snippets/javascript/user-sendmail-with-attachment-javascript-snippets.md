---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 116c78b298b15be3c1477cd3528e5f913381b586
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  message: {
    subject: 'Meet for lunch?',
    body: {
      contentType: 'Text',
      content: 'The new cafeteria is open.'
    },
    toRecipients: [
      {
        emailAddress: {
          address: 'meganb@contoso.onmicrosoft.com'
        }
      }
    ],
    attachments: [
      {
        '@odata.type': '#microsoft.graph.fileAttachment',
        name: 'attachment.txt',
        contentType: 'text/plain',
        contentBytes: 'SGVsbG8gV29ybGQh'
      }
    ]
  }
};

await client.api('/me/sendMail')
    .version('beta')
    .post(sendMail);

```