---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d870fe56c8a83a6eca27b56b00484acd0fe60116493b3db4cc00cf86b70a264
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57370442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailTips = {
    EmailAddresses: [
        'danas@contoso.onmicrosoft.com', 
        'fannyd@contoso.onmicrosoft.com'
    ],
    MailTipsOptions: 'automaticReplies, mailboxFullStatus'
};

await client.api('/me/getMailTips')
    .version('beta')
    .post(mailTips);

```