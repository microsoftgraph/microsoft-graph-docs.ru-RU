---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7f546f627d75e1cc78b482b4a14d19e5394a1124
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  ToRecipients:[
      {
        emailAddress: {
          address:"danas@contoso.onmicrosoft.com",
          name:"Dana Swope"
        }
      }
     ],
  Comment: "Dana, hope you can make this meeting." 
};

let res = await client.api('/me/events/{id}/forward')
    .version('beta')
    .post(forward);

```