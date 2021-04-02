---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fbcb15077fa0c9e2d49d3e0210aa2e0db8bfee0a
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
    displayName: 'My Private notebook'
};

await client.api('/me/onenote/notebooks')
    .version('beta')
    .post(notebook);

```