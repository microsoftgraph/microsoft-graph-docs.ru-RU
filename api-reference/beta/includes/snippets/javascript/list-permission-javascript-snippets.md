---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 147899a50857609aa0cc2b39da2a7e5aee54299fcefc2eb58ecef1a901974c4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissions = await client.api('/sites/{sitesId}/permissions')
    .version('beta')
    .get();

```