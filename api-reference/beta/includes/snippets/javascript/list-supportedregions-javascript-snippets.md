---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f817933b14dd5b53c4b51f825c02ff951e16a198
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedRegions = await client.api('/deviceManagement/virtualEndpoint/supportedRegions')
    .version('beta')
    .get();

```