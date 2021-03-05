---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fbe64b8be87843ce6c04e3f2fac5a9ff20a1e274
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473554"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workingHours = await client.api('/me/mailboxSettings/workingHours')
    .get();

```