---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 818c872ec4e8cacc9786bdc07aefcc865c5b00e5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/namedLocations')
    .version('beta')
    .filter('microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq \'CA\')')
    .get();

```