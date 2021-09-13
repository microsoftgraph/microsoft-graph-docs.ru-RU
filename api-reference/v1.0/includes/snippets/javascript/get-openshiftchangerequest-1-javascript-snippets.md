---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4357fc16dcd75fd1950c003e251ac2a92e027dbdff275436591f0998f020a846
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57319377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShiftChangeRequest = await client.api('/teams/{id}/schedule/openShiftChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09')
    .get();

```