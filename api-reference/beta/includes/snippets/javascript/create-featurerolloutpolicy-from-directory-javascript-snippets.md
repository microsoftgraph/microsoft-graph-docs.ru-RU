---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7888446aa4b08c8f2c1252a072e0bb035908428
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const featureRolloutPolicy = {
  displayName: 'PassthroughAuthentication rollout policy',
  description: 'PassthroughAuthentication rollout policy',
  feature: 'passthroughAuthentication',
  isEnabled: true,
  isAppliedToOrganization: false
};

await client.api('/directory/featureRolloutPolicies')
    .version('beta')
    .post(featureRolloutPolicy);

```