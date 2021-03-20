---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 436124c8e4f3e424fad0c65df27156e421a8b336
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950639"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profile = await client.api('/me/profile')
    .version('beta')
    .get();

```