---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2899eb059960ceffd96d0d8dfcc1d97e27b7f22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/homeRealmDiscoveryPolicies/{id}/appliesTo')
    .version('beta')
    .get();

```