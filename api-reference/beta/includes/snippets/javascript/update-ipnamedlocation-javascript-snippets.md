---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 721dd7f87a9defcb6ac5f22658e551aa92868e39
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779414"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    '@odata.type': '#microsoft.graph.ipNamedLocation',
    displayName: 'Untrusted named location with only IPv4 address',
    isTrusted: false,
    ipRanges: [
        {
            '@odata.type': '#microsoft.graph.iPv4CidrRange',
            cidrAddress: '6.5.4.3/18'
        }

    ]
};

await client.api('/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .version('beta')
    .update(namedLocation);

```