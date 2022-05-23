---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 107a9938968254cad9b641b6f4cf73ac1ac3fc83
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getSubscriptions = await client.api('/deviceManagement/virtualEndpoint/snapshots/getSubscriptions')
    .version('beta')
    .get();

```