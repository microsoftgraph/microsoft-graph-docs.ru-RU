---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ad8f876946470caf590c868ae1f6a25bfc231797
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "47414056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  @odata.id:"https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/servicePrincipals/{id}/claimsMappingPolicies/$ref')
    .version('beta')
    .post(claimsMappingPolicy);

```