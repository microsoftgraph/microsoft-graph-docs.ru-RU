---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88fb72830e00c39488c732472a4785da123deeb83dce6a184f7ee28ff2bec6fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196648"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
  isLanguageCustomizationEnabled: true,
  defaultLanguageTag: 'en',
};

await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp')
    .version('beta')
    .update(b2cIdentityUserFlow);

```