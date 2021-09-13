---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b99a76f0a81af5f6d85b79c01d84b240ff98ccb793f74b0f663c61c3bb80f1ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57314100"
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