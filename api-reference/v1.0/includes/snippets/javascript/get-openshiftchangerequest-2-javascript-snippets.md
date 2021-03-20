---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a8214dc06586fff37f9614bfba1ecb78553f32db
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShiftChangeRequests = await client.api('/teams/{id}/schedule/openShiftChangeRequests')
    .get();

```