---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8c3cb009fe8e343a35033cf542cb93dadd252e86
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let services = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services')
    .version('beta')
    .get();

```