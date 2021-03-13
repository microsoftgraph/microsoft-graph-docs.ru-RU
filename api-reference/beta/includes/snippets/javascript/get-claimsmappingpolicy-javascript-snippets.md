---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 314dfa223e77c2a12d1ac07a5fb9e3082d601e08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786121"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicy = await client.api('/policies/claimsMappingPolicies/{id}')
    .version('beta')
    .get();

```