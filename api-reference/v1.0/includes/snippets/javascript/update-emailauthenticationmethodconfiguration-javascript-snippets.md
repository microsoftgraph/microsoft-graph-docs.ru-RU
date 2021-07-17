---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 851cc13f362e45c6ddeafafdb45127f8df370ae2
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442912"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  '@odata.type': '#microsoft.graph.emailAuthenticationMethodConfiguration',
  allowExternalIdToUseEmailOtp: 'enabled',
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .update(authenticationMethodConfiguration);

```