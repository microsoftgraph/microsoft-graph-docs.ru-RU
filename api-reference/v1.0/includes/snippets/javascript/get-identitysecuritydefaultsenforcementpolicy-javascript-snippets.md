---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e1a68a415fb714f34d780379168e30b0d1f2d29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identitySecurityDefaultsEnforcementPolicy = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .get();

```