---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f102e53bece8b8d53af5b70600b64e6df8aa42e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let emails = await client.api('/me/profile/emails')
    .version('beta')
    .get();

```