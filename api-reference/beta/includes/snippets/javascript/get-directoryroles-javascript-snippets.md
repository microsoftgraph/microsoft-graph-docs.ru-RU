---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce308089d129c99a5a6d898381a2b5762ad5312c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoles = await client.api('/directoryRoles')
    .version('beta')
    .get();

```