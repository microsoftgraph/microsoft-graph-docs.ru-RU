---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ccf0e863dfdfd5d18521d9d2be25a0d6203dbbb5b44ad2239b08884ca8342e25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateAdDomainPassword = {
  adDomainPassword: 'AdDomainPassword value'
};

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword')
    .version('beta')
    .update(updateAdDomainPassword);

```