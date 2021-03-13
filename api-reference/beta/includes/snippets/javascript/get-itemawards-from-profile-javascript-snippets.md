---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5b6ee8c4f3cadee40247a2db07a71d01a8e28863
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let awards = await client.api('/me/profile/awards')
    .version('beta')
    .get();

```