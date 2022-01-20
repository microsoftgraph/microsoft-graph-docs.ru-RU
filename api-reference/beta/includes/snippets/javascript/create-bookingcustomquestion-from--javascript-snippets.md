---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6c1ae33d59173d076d6764529c483348228ab1b9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106905"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomQuestion = {
  '@odata.type': '#microsoft.graph.bookingCustomQuestion',
  displayName: 'What is your age?',
  answerInputType: 'text',
  answerOptions: []
};

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/3bc6fde0-4ad3-445d-ab17-0fc15dba0774')
    .version('beta')
    .post(bookingCustomQuestion);

```