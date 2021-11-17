---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 802973bef0902bd621ad35dd008a0ede098ed4f5c9339b7e51a926fb4536de8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57371538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarGroups = await client.api('/me/calendarGroups')
    .version('beta')
    .get();

```