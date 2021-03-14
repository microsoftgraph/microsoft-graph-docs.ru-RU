---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a34c9925ceeb2334a3096d160c88d28c9ff39d9f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversations = await client.api('/groups/{id}/conversations')
    .get();

```