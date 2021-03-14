---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 334d5c435574dbc370f9029bf4a5b44dff32504e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'Approved!'
};

await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve')
    .post(approve);

```