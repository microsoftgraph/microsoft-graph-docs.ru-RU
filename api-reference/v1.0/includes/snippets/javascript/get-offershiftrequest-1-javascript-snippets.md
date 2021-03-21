---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49907163eb0c8374bf8bcabad99022b689c59ec5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequest = await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}')
    .get();

```