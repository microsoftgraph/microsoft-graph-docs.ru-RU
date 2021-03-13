---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bea945a9190920812e21f39f1c8d6a25e3781e70
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sharedWithMe = await client.api('/me/drive/sharedWithMe')
    .version('beta')
    .get();

```