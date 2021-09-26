---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 56de769946402d5abda82e0b3b24913a21ceee12
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766577"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let samlOrWsFedExternalDomainFederation = await client.api('/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation')
    .version('beta')
    .filter('domains/any(x: x/id eq \'contoso.com\')')
    .get();

```