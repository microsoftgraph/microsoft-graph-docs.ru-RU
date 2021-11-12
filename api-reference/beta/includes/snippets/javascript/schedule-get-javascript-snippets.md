---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 62739b3b2f1eca2a1d86f41231a256e25702f3690060bcdc87ff8f90ae998dec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedule = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .get();

```