---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d176f0b3333d62e58c6883647a6a8d7221e24ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendars = await client.api('/me/calendarGroups/{id}/calendars')
    .get();

```