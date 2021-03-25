---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0a5940aec6c5433acfba81c7e0e580c9eb5f53ae
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const featureRolloutPolicy = {
  displayName: 'PasswordHashSync Rollout Policy',
  description: 'PasswordHashSync Rollout Policy',
  isEnabled: true,
  isAppliedToOrganization: false
};

await client.api('/policies/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a')
    .update(featureRolloutPolicy);

```