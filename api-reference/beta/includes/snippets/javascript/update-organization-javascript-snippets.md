---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dbb88784eed0d05a66a2bd7e0e502d0358637887
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organization = {
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      contactEmail:"alice@contoso.com",
      statementUrl:"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
};

let res = await client.api('/organization/{id}')
    .version('beta')
    .update({organization : organization});

```