---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d54e50bb0d327fff75c31f8af75098d67892fac3face1946bfa7784409c0339f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57373356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    '@odata.type': '#microsoft.graph.fido2AuthenticationMethodConfiguration',
    state: 'enabled',
    isAttestationEnforced: 'true'
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .update(authenticationMethodConfiguration);

```