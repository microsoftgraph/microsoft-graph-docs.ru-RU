---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64d16208446b42f99fa9b62dfb061a65ffea2044e9d37fcbd1254342c938fbd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userAccountInformation = {
  countryCode: 'NO'
};

await client.api('/me/profile/account/{id}')
    .version('beta')
    .update(userAccountInformation);

```