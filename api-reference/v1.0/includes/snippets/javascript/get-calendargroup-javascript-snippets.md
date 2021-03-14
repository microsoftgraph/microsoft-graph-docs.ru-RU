---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d0a2e2f53d29bf0bd553dadc99612cbacf010c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800389"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarGroup = await client.api('/me/calendarGroups/{id}')
    .get();

```