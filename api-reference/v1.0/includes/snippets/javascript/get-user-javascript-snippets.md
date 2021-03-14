---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 77677a55aa0a6816c3a646b4f72f66c8567baee3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/me')
    .get();

```