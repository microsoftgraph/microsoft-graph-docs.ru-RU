---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0496463013c917068a0505d14590957a96e2a5b9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: 'Cooking'
};

await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=/taskfolders')
    .version('beta')
    .post(outlookTaskFolder);

```