---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba3ffff59183bec1f197c4a3e1850e758d817c51
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/tasks/{id}')
    .delete();

```