---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f57cf469610976210666370ea79544755293329
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790432"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    '@odata.type': '#microsoft.graph.countryNamedLocation',
    displayName: 'Named location with unknown countries and regions',
    countriesAndRegions: [
        'US',
        'GB'
    ],
    includeUnknownCountriesAndRegions: true
};

await client.api('/identity/conditionalAccess/namedLocations')
    .version('beta')
    .post(namedLocation);

```