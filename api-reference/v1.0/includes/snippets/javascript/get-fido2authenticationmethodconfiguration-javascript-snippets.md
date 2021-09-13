---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3e7f140508b71f0b3c805672576715eae520f0334204e4ff4d85527c44806065
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57262177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .get();

```