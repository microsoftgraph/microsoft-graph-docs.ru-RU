---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4360d431ccaacde4e550eb3cea1165ca971d175e2127fb5c876ab48a2dc24156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57207571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let swapShiftsChangeRequests = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests')
    .version('beta')
    .get();

```