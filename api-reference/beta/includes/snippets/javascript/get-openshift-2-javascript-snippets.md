---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9f4087921950099d8a664d0d45bee87613c2e27a65470ccd1e1108084ba421db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143854"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShifts = await client.api('/teams/{id}/schedule/openShifts')
    .version('beta')
    .get();

```