---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb4553bdcfbd9f09083e310257a7fc989789a615
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43061951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .version('beta')
    .get();

```