---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3ba7f9c70f6c802000ab048a1b11c90e7f546fee
ms.sourcegitcommit: 53a57f19a5b16029b540e61ddfba6c2b4e45cfc5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2020
ms.locfileid: "35708723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}')
    .version('beta')
    .delete();

```