---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46dd6f485c8dc34626c2fa3206387204e043eabff8c4ceefa2344c30c1dbd75e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57312291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  Message: {
    subject: 'Project kickoff',
    toRecipients: [
      {
          emailAddress: {
              name: 'Samantha Booth',
              address: 'samanthab@contoso.onmicrosoft.com'
          }
      }
    ],
    mentions: [
      {
        mentioned: {
          name: 'Dana Swope',
          address: 'danas@contoso.onmicrosoft.com'
         }
      }
    ]
  }
};

await client.api('/me/sendMail')
    .version('beta')
    .post(sendMail);

```