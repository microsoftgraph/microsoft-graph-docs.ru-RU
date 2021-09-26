---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c4bcbf21297425e15f507eef172a2514d5e75f072ef5e5ce92dd324d194aaff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57054113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcDeviceImage = await client.api('/deviceManagement/virtualEndpoint/deviceImages/{id}')
    .version('beta')
    .get();

```