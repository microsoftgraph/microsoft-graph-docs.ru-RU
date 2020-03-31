---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a31ebe8947a4fa75cf2f43aa157fccbc6524ee32
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062451"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/namedLocations')
    .version('beta')
    .filter('microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')')
    .get();

```