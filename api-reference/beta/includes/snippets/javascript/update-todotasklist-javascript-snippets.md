---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d3d8c11eeac3827df1c3f3ca5abf929a2bf2d46b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: 'Vacation Plan'
};

await client.api('/me/todo/lists/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update(todoTaskList);

```