---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: caae7b960be7d9db4e68c37cfe57f9b1a70b1d7d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118055"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
    customSecurityAttributes: 
    {
        Engineering: 
        {
            '@odata.type':'#Microsoft.DirectoryServices.CustomSecurityAttributeValue',
            ProjectDate: '2022-10-01'
        }
    }
};

await client.api('/users/{id}')
    .version('beta')
    .update(user);

```