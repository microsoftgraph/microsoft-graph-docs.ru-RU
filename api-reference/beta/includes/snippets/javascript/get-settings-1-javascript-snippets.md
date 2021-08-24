---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5eb54eb2c4480193fbf1f077ffdd685a992686d0b46ef9e8f4284891a7adef07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57321305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let settings = await client.api('/settings')
    .version('beta')
    .get();

```