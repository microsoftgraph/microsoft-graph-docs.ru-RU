---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fbe346e68810f4f3167df31085a54426786a9d00
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50035769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors')
    .version('beta')
    .get();

```