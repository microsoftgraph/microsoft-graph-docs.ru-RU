---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 447b7e3d9cf6d3d081edcc27038abffe8c0d75f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782087"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identitySecurityDefaultsEnforcementPolicy = {
  isEnabled: false
};

await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .update(identitySecurityDefaultsEnforcementPolicy);

```