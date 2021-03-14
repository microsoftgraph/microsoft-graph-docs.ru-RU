---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dd834f2dc3489566de3c1f47d6c85a23152a3237
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let automaticRepliesSetting = await client.api('/me/mailboxSettings/automaticRepliesSetting')
    .get();

```