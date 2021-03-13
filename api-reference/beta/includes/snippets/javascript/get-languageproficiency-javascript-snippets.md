---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a87566dc177e72aeef2046f79057c66f9298b27c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787268"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languageProficiency = await client.api('/me/profile/languages/{id}')
    .version('beta')
    .get();

```