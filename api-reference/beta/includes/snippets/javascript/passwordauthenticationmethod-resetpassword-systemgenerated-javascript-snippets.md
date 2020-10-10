---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 313f1e16de284cc3442a25722b661473fb806abe
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword')
    .version('beta')
    .post();

```