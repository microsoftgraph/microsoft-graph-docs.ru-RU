---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92fb5832110acefd66b0f0b7182a03a5f9a19eb7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userAccountInformation = {
  allowedAudiences: 'organization',
  countryCode: 'NO',
};

await client.api('/me/profile/account')
    .version('beta')
    .post(userAccountInformation);

```