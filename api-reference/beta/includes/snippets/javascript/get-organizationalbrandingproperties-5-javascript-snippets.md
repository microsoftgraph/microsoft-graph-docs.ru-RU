---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 91b137c85580d250e1e6a75d1e257dc7ff1c71f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo')
    .version('beta')
    .header('Accept-Language','fr')
    .get();

```