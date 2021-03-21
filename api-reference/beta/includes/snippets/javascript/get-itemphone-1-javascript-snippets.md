---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb4a01e5a0dd80762021b77bf21669628ff124d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPhone = await client.api('/me/profile/phones/{id}')
    .version('beta')
    .get();

```