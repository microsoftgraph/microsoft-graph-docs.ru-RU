---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 10abe57f1fdcc2a256e83d1931d12f697483cae9
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
  isLanguageCustomizationEnabled: true,
  defaultLanguageTag: "en",
};

let res = await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp')
    .version('beta')
    .update(b2cIdentityUserFlow);

```