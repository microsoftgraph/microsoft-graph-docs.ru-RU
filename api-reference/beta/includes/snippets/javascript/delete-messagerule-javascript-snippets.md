---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 05a71917a5d6e9a605c391cef7f4ef0401997ecb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')')
    .version('beta')
    .delete();

```